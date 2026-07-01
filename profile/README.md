<div align="center">

![http4k — Server as a Function](github-banner.png)

# The functional toolkit for Kotlin

**Server as a Function.** We meant it literally — no annotations, no reflection,
no container, no magic. Just immutable Kotlin functions you can read, test
in-memory, and trust in production.

[Website](https://http4k.org) · [Quickstart](https://http4k.org/quickstart) · [Docs](https://http4k.org/ecosystem/http4k) · [News](https://http4k.org/news)

</div>

---

## One platform. Four ecosystems. 200+ modules.

Everything ships under a single BOM version, so it just works together — pull
in only what you need.

| | |
|---|---|
| 🧩 **Core** | Servers, clients, routing, typesafe lenses, formats & a full testing toolkit. Zero dependencies. |
| 🤖 **AI** | LLM adapters, MCP and A2A — with Fakes so you can test AI integrations offline. |
| 🔌 **Connect** | Typed clients for cloud & SaaS APIs, each with a stateful in-memory Fake. |
| 🛡️ **Pro & Enterprise** | Premium modules, LTS, priority support and verifiable supply-chain security. |

## Why teams pick http4k

- **Testable** — call your whole app in-memory, no server, no ports.
- **Portable** — swap Netty → Lambda → GraalVM with one line.
- **Transparent** — what you read is exactly what runs. Zero reflection.
- **Proven** — 5M+ downloads/month, in production since 2017.

## Get started

```kotlin
val app: HttpHandler = { req -> Response(OK).body("hello ${req.query("name")}") }
app.asServer(SunHttp(9000)).start()
```

## Security

We do our security homework in public — see our [advisories](https://http4k.org/security)
and [coordinated disclosure policy](https://github.com/http4k/http4k/security/policy).

---

<div align="center">

**Apache 2.0 core** · Built & maintained by http4k Ltd

*Peace out. // the http4k team*

</div>
