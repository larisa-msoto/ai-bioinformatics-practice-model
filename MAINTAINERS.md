# Maintainer guide

Internal notes for people with merge rights on this repository. Not part of the
published site.

## Acknowledging contributions

Every contribution gets credited on the [contributors page](docs/contributors.md).
The page is maintained by the [all-contributors](https://allcontributors.org) bot:
you never edit the table by hand. You post one comment and merge the pull request
the bot opens.

### When to credit someone

Credit a person the first time they do any of the following. You do not need to
credit them again for later contributions of the same kind, but adding a new
contribution type to an existing person is fine and encouraged.

- A merged pull request (content, wording, fixes, structure).
- A reported issue that led to a change.
- A substantive review of someone else's pull request.
- A discussion post that shaped the model, a workshop or course built on it, or
  an entry in the AI Errors Archive that was folded back into the content.
- Design, tooling, or infrastructure work on the repo or site.

If in doubt, credit. The cost of an extra name is nothing; the cost of a missed
one is a discouraged contributor.

### How to credit someone

Comment on the relevant issue or pull request:

```text
@all-contributors please add @username for content, ideas
```

Add more than one person or type in a single comment:

```text
@all-contributors please add @alice for content, and @bob for review, bug
```

The bot replies, then opens a pull request that updates `.all-contributorsrc`
and the table in `docs/contributors.md`. Check it looks right and merge it. The
`ci` workflow redeploys the site on merge to `main`.

### Contribution types used in this project

`all-contributors` defines many keys; these are the ones that fit 4D-Bio. Use the
key (the left column) in the comment. The full list is at
<https://allcontributors.org/docs/en/emoji-key>.

| Key           | Use it for                                                        |
|---------------|------------------------------------------------------------------|
| `content`     | Writing or revising practice-model content                       |
| `ideas`       | Concept, framing, structure, planning, feedback                  |
| `doc`         | Contributing guide, README, code of conduct, other docs          |
| `review`      | Reviewing a pull request                                         |
| `bug`         | Reporting a problem that led to a change                         |
| `example`     | A workshop, course, or curriculum built on the model             |
| `data`        | Contributing to the AI Errors Archive or other collected data    |
| `maintenance` | Repo, CI, site build, dependency and release upkeep             |
| `design`      | Visual design, the BioinfoPro design system work                 |
| `tool`        | Tooling, such as the model-mapper tool                           |

### If the bot does not respond

The bot is a GitHub App that must stay installed on the repo
(<https://github.com/apps/allcontributors>). If a comment gets no reply within a
few minutes, or you want to backfill several people at once, do it from a
checkout instead:

```bash
npx all-contributors add <username> <types>   # e.g. npx all-contributors add alice content,ideas
npx all-contributors generate                 # rewrites docs/contributors.md from .all-contributorsrc
```

Commit both `.all-contributorsrc` and `docs/contributors.md` in the same pull
request. You can also hand-edit the `contributors` array in `.all-contributorsrc`
and run `generate`; never hand-edit the marked block in `docs/contributors.md`.

## Pull request checklist

Before merging a content pull request:

- [ ] Changes are accurate and fit the practice model.
- [ ] No em dashes; sentence-case headings; no emoji outside the sanctioned
      exceptions (source pills, the contributors table).
- [ ] Links resolve and `mkdocs build` is clean.
- [ ] The contributor is queued for an `@all-contributors` comment.
