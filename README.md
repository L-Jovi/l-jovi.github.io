# Blog

This blog relies on hexo for implementation :)

[Home Page](https://l-jovi.github.io)

## Document dates and language

Keep an existing document's language and declared timezone. New calendar dates
must have an explicit `date_timezone` or a clear local scope; preserve day-only
precision instead of inventing midnight. Precise timestamps need a UTC offset
or `Z`. The team's UTC+08:00 region name is `Asia/Singapore`; a new document may
use another explicit suitable zone. Conversation or host timezone changes do
not migrate documents or existing schedules. Preserve source-specific dates,
native schemas and sealed bytes; record legacy interpretations outside an
immutable artifact.

## Blog date interpretation

`_config.yml` declares `Asia/Singapore` for Hexo's existing local date values.
Post/page frontmatter now repeats that region as `date_timezone` so standalone
source files remain interpretable. Original `date` values and prose are kept;
the added field documents their context and does not replace Hexo's parser
configuration. Upstream theme documentation retains its own source dates.
