# BROCS

**Build, Run, Observe, Control, Secure.** The five parts of the surface an organization
must cover to adopt AI seriously.

BROCS is a vendor-neutral framework. It is not a product and nothing about it is for
sale. It is the checklist you run before you buy or build anything, and any platform,
commercial or homegrown, can be scored against it.

Canonical home: **[brocs.fyi](https://brocs.fyi/)**

| Letter | One line | Roots |
|---|---|---|
| **B**uild | Enable people to make things: tools, access, keys, data | DevOps, DORA, platform engineering |
| **R**un | The runtime: apps, databases, secrets, provisioning, portability | SRE, PaaS, hybrid cloud |
| **O**bserve | Metrics, traces, alerts, exposed to the people who own the thing | Observability, control theory |
| **C**ontrol | Configuration, ingress, identity, storage, routing | Control theory, ClickOps to GitOps |
| **S**ecure | Governance, agent oversight, shadow AI, cost, compliance | SecOps, GRC, FinOps |

## Why it exists

Most AI products cover one part of that surface and push the other four onto "your
infrastructure" or "your governance tooling". Customers integrate across three to five
products, contracts, and audit processes, the integration cost eats the productivity
gain, and a reasonable executive concludes AI does not work for the enterprise. That is
not the lesson the experience actually teaches.

BROCS gives the whole surface a vocabulary, so buyers and builders can name what they
are missing before they find out the expensive way.

## What is in this repository

- [`data/letters.yaml`](data/letters.yaml) — the five letters: names, taglines,
  verticals, handoffs, and the colour each one carries.
- [`data/failures.yaml`](data/failures.yaml) — the failure-mode library. Public
  incidents, each mapped to the letter that was skipped, each with a source you can
  check.
- [`data/glossary.yaml`](data/glossary.yaml) — the vocabulary, defined tersely.
- [`data/assessment.yaml`](data/assessment.yaml) — the twenty statements behind the
  scoreline.

These are the same files that drive [brocs.fyi](https://brocs.fyi/). The site reads
them; nothing is restated by hand.

## Contribute a failure mode

The library grows by contribution. The bar is a **public source** and an **arguable
mapping** to a letter. Open an issue with the
[failure-mode template](https://github.com/brocs-org/brocs/issues/new?template=failure-mode.yml),
send a pull request against `data/failures.yaml`, or write to
[failures@brocs.fyi](mailto:failures@brocs.fyi) if a public issue is not where you want
to tell the story.

Anonymised war stories from your own organization are welcome as discussion, but they
will not go in the library without something a reader can check.

## Disagree

If a letter is wrong, the framework should change. Open an issue. A framework that
survives only among people who already agree with it is not a framework, it is a
preference.

## Score yourself

Twenty statements, four per letter, at
[brocs.fyi/resources/assessment](https://brocs.fyi/resources/assessment/). It produces a
scoreline like `B3 R2 O1 C2 S0`. Zero is a common and honest answer for a letter nobody
owns yet.

## For machines

- [brocs.fyi/llms.txt](https://brocs.fyi/llms.txt) — the framework, the definitions, the
  page map
- [brocs.fyi/llms-full.txt](https://brocs.fyi/llms-full.txt) — every page, full text, one
  file
- Any page plus `index.md` — that page as raw Markdown

## Licence

The framework text is [CC BY 4.0](LICENSE). Copy it, translate it, quote it, put it on
your own slides, train on it. Attribution to Leo Mata and brocs.fyi is the only ask.

Coined by [Leo Mata](https://leomata.com/). Origin essay:
[leomata.com/blog/brocs](https://leomata.com/blog/brocs/).
