<!-- 日本語版: [README.ja.md](./README.ja.md) — 片方を直したら、同じコミットでもう片方も直してください -->

# hora-ort-sample-spec

Sample spec documents that [Hora Kit](https://github.com/openreachtech/hora-core) generated, for small applications built with it.

## What is here

Each directory is one application, and holds the spec exactly as `/hora-spec` wrote it:

```
<application>/
  specs/<version>/spec.md     the spec, written one approved section at a time
  README.md                   what the application does, and what it took to write
  README.ja.md                the same, in Japanese
```

**Nothing here is written after the fact.** A spec in this repository is the document a run actually produced — that is the whole point of publishing it. Where a line reads oddly, it reads oddly in the real one too.

## What a reader gets from it

- **What a Hora Kit spec looks like when it is finished** — the sections, the level of detail each one carries, and how acceptance criteria are phrased so that a gate can check them.
- **How much of it is decided in conversation.** `/hora-spec` asks, proposes and writes only what was approved, so a finished spec is the record of those answers.
- **A size to calibrate against.** These are applications small enough to finish in a day, so the spec is short enough to read end to end.

## Where the machinery is documented

| | |
|---|---|
| what each command does | [`commands.md`](https://github.com/openreachtech/hora-core/blob/main/docs/commands.md) in `hora-core` |
| how work gets executed | [`architecture.md`](https://github.com/openreachtech/hora-core/blob/main/docs/architecture.md) in `hora-core` |
| the format a spec is written in | [`spec-format.md`](https://github.com/openreachtech/hora-core/blob/main/kit/skills/hora/references/spec-format.md) |
| starting a project with the kit | [`hora-boilerplate`](https://github.com/openreachtech/hora-boilerplate) |

## Contribution

A sample lands here as a pull request that adds one directory: the generated spec, and a README saying what the application does. Nothing else is edited into it.

## License

This project is released under the Apache License 2.0.

For more details, please see [in the LICENSE file](./LICENSE).

## Developer

[Open Reach Tech Inc.](https://openreach.tech)

## Copyright

© 2026 Open Reach Tech Inc.
