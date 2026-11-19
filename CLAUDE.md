# CLAUDE.md

This repo holds `index.md`, a summary of zcorpan's (Simon Pieters) GitHub activity for Mozilla, grouped by theme with markdown links to every PR/issue cited.

## Gathering data for a period

Set `RANGE` to the period, e.g. `2026-01-01..2026-12-31` or `2026-07-01..2026-09-30`.

Authored PRs:

```bash
gh search prs --author=@me --created=$RANGE --limit 300 \
  --json repository,title,url,state,createdAt \
  --jq '.[] | "\(.repository.nameWithOwner)\t\(.state)\t\(.createdAt[:10])\t\(.title)\t\(.url)"' | sort
```

Authored issues:

```bash
gh search issues --author=@me --created=$RANGE --limit 300 \
  --json repository,title,url,state,createdAt \
  --jq '.[] | "\(.repository.nameWithOwner)\t\(.state)\t\(.createdAt[:10])\t\(.title)\t\(.url)"' | sort
```

Reviewed PRs by others. `--updated` also matches older PRs that were reviewed before the period, so check the review date (`gh pr view <url> --json reviews`) before citing one:

```bash
gh search prs --reviewed-by=@me --updated=$RANGE --limit 300 \
  --json repository,title,url,author \
  --jq '.[] | select(.author.login!="zcorpan") | "\(.repository.nameWithOwner)\t\(.author.login)\t\(.title)\t\(.url)"' | sort
```

Commits (default branches only; commits pushed to other people's PR branches don't show up):

```bash
gh search commits --author=zcorpan --author-date=$RANGE --limit 200 \
  --json repository,commit --jq '.[] | "\(.repository.fullName)\t\(.commit.message|split("\n")[0])"' | sort
```

Standards-positions participation:

```bash
gh search issues --commenter=zcorpan --repo mozilla/standards-positions --updated=$RANGE --limit 100 \
  --json title,url --jq '.[] | "\(.title)\t\(.url)"'
```

The search API caps results at 1000 per query. For long periods, split the range.

## What to include

- Omit clearly personal projects: `zcorpan/html-parser-book`, `zcorpan/.claude`.
- Mozilla work starts 2022-11-15; earlier activity (Bocoup) is out of scope.
- Group by theme (e.g. Sanitizer/streaming parsing, media elements, navigation, spec infrastructure, standards positions), not by repo.
- Link every cited item. Label links `repo#N` (`whatwg/html#12492`, `wpt#60210`); in a list that already names the repo, `#N` is enough.
- Keep the caveats section: it records what the data misses (Bugzilla, Phabricator, non-default-branch commits).

## Format

Markdown with a `#` title, one `##` per year (newest first), and nested bullet lists. The `## Caveats` section stays last. Mark the current year as partial, e.g. `## 2026 (through September)`.

From 2026 on, split each year into `### H2` before `### H1`, with one `####` per theme inside each half; a topic spanning both halves gets a theme in each. Halves are calendar halves (July–December and January–June), headed just `### H2` and `### H1`. An item goes in H2 only if all of zcorpan's GitHub activity on it that year is dated July 1 or later (creation for zcorpan's own PRs/issues, review or comment dates otherwise); otherwise it stays in H1. Cite examples from the right half for summary bullets without links of their own (e.g. "many reviews of Anne's PRs"). Years before 2026 keep one `###` per theme.
