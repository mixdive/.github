<h1 align="center">
  <img src="https://mixdive.com/assets/logo/png/icon-color-512.png" width="72" alt="">
  <br>mixdive.
</h1>

<p align="center">
  <b>Self-hosted product analytics. Your events, your reports, your servers.</b><br>
  Send an event, and its report screen is already there.
</p>

<p align="center">
  <a href="https://mixdive.com/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=header">Website</a> ·
  <a href="https://docs.mixdive.com/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=header">Documentation</a> ·
  <a href="https://docs.mixdive.com/start/demo/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=header">Live demos</a> ·
  <a href="https://hub.docker.com/r/mixdive/mixdive">Docker Hub</a> ·
  <a href="https://github.com/orgs/mixdive/projects/1">Roadmap</a>
</p>

[![The Mixdive console: the events list, with every event a product sends, its counts and its unique users](https://mixdive.com/assets/video/hero-console-poster.webp)](https://mixdive.com/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=hero)

<p align="center"><i>The console, running on your own server. <a href="https://demo-ecommerce.mixdive.com/">Open the online store demo</a> and click through it.</i></p>

## Insight or ownership? You shouldn't have to choose

Most analytics tools ask you to pick one. Ship your users' behaviour to
somebody else's servers, or work blind. Mixdive is the third answer: the same
reports, on a machine you control.

**Your usage data never leaves your infrastructure.** No vendor keeps a copy of
who your users are or what they did. Teams in regulated industries, and anyone
whose data simply cannot go to a third party, tend to arrive for exactly this
reason.

**Nothing to define first.** Send an event and its report screen exists.
Properties register themselves the first time they show up, so a new field
becomes a breakdown you can look at instead of a ticket for somebody else.

**One container and a MongoDB.** That is the whole architecture. No Kafka, no
ClickHouse, no warehouse to feed. A small VM carries more than you would guess.

**You don't need a data team.** The screens answer what a product person
actually asks: which features get used, by whom, how often, and what people did
before they stopped.

## Try it in a minute

```bash
curl -O https://docs.mixdive.com/compose.yaml
docker compose up -d
```

That brings up Mixdive, a MongoDB with a persistent volume, and a proxy in
front of both. Open `http://localhost:8080` and a one-time wizard asks for a
project name, the address your apps will use, and an owner account.

Prefer to look before you install? Three demos run with made-up companies'
data in them, no sign-up needed:
[an online store](https://demo-ecommerce.mixdive.com/),
[a bank](https://demo-banking.mixdive.com/) and
[a software company](https://demo-saas.mixdive.com/).

Start here:
[Quick start](https://docs.mixdive.com/start/quick-start/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=quickstart)
·
[Install](https://docs.mixdive.com/operate/install/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=install)
·
[Concepts](https://docs.mixdive.com/concepts/events/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=concepts)

## Sending data

| | |
|---|---|
| [**Web tag**](https://docs.mixdive.com/integrations/web-tag/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=integrations) | One line on your site. Visitors, sessions and page views count themselves. |
| [**React**](https://docs.mixdive.com/integrations/react/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=integrations) | A provider, a hook, router-driven page views. |
| [**Next.js**](https://docs.mixdive.com/integrations/nextjs/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=integrations) | One line in the root layout, plus events from Server Actions and Route Handlers. |
| [**Node.js**](https://docs.mixdive.com/integrations/node/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=integrations) | Events, profiles and records from JavaScript servers and edge functions. |
| [**Go SDK**](https://docs.mixdive.com/integrations/go-sdk/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=integrations) | Fire-and-forget tracking from your backend. |
| [**Google Tag Manager**](https://docs.mixdive.com/integrations/google-tag-manager/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=integrations) | A gallery template, no code deploy. |
| [**HTTP API**](https://docs.mixdive.com/integrations/http-api/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=integrations) | Anything that can POST JSON. |

More SDKs are coming. If yours is missing, write to hello@mixdive.com and it
moves up the list.

## Repositories here

| Repository | What it is |
|---|---|
| [mixdive-js](https://github.com/mixdive/mixdive-js) | The JavaScript SDKs: [`@mixdive/browser`](https://www.npmjs.com/package/@mixdive/browser) for any website, [`@mixdive/react`](https://www.npmjs.com/package/@mixdive/react) for React apps, [`@mixdive/next`](https://www.npmjs.com/package/@mixdive/next) for Next.js and [`@mixdive/node`](https://www.npmjs.com/package/@mixdive/node) for servers. |
| [mixdive-go](https://github.com/mixdive/mixdive-go) | The Go SDK. Fire-and-forget, zero dependencies. |
| [mixdive-gtm](https://github.com/mixdive/mixdive-gtm) | The Google Tag Manager tag template. |
| [feedback-platform](https://github.com/mixdive/feedback-platform) | The Feedback Portal: open-source, self-hosted feedback with voting and a changelog. |
| [mixdive-feedback-go](https://github.com/mixdive/mixdive-feedback-go) | The Feedback Portal's Go SDK, for signing your users into the portal. |

The SDKs and the tag template are Apache-2.0. The Feedback Portal is MIT. The
Mixdive server itself is a commercial product, free to run on your own
servers, and its image is public on
[Docker Hub](https://hub.docker.com/r/mixdive/mixdive).

## Follow along

Mixdive is built in the open, and the board below is the one the work actually
comes off.

- [Public roadmap](https://github.com/orgs/mixdive/projects/1)
- [Devlog](https://mixdive.com/blog/?utm_source=github&utm_medium=referral&utm_campaign=org_profile&utm_content=devlog) on mixdive.com
- [Email updates](https://buttondown.com/mixdive) when something ships
- [@mixdive on X](https://x.com/mixdive) · [LinkedIn](https://www.linkedin.com/company/mixdive)

Running a real product with data that cannot go to a third party? A few lines
to hello@mixdive.com is enough, and a person answers.

---

**Also from Mixdive:** the [Feedback Portal](https://feedback.mixdive.com), a
self-hosted place for your customers to submit and vote on feedback, with an
admin console for triage, releases and a public changelog.
