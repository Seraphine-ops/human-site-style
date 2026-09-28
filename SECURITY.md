# Security

## What this skill can do

It's plain Markdown. There are no scripts, no dependencies and nothing that runs on install. When you use it, Claude reads the files as instructions and follows them while it writes your site.

It doesn't tell Claude to fetch URLs, run commands or handle credentials. The reference notes list real websites by name, but only as descriptions. Nothing from those sites is copied or loaded.

## The real risk: changed instructions

Anything in these files ends up in Claude's context, so a tampered copy could slip in instructions you didn't expect, such as adding a tracking script or sending form data somewhere. To avoid that:

- Install from this repository, not a re-upload.
- Read the diff before you pull an update. Everything is short enough to review by eye.
- If a fork adds scripts or asks for network access, treat it as a different project and review it properly.

## Sites built with it

The skill only covers design and copy. It doesn't make a site secure. Check the usual things yourself before going live: HTTPS, form handling and spam protection, cookie consent, and any third-party scripts such as analytics or booking widgets.

## Reporting a problem

If you find something in this repo that could make Claude do something harmful, report it privately through the Security tab ("Report a vulnerability") instead of opening a public issue.
