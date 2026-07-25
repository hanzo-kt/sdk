# LLM.md — Hanzo Kotlin SDK

**What this is:** the Full Cloud SDK for Kotlin — a coroutine-native client
covering the entire Hanzo `/v1` cloud surface, for the JVM and Android. Canonical
home: `hanzo-kt/sdk`. Coordinate: `ai.hanzo:sdk`. Package: `ai.hanzo.sdk`.

**Generated, not hand-written.** Code-generated from the Hanzo OpenAPI spec
(`~/work/hanzo/openapi/hanzo.yaml`, `info.version` 8.0.0) with
`openapi-generator` (`kotlin`, `library=jvm-okhttp4`, `useCoroutines=true`).
**Never hand-fork the generated code** — regenerate from the spec. The generator's
own README (endpoint + model index) is preserved as `GENERATED.md`; per-endpoint
docs live in `docs/`.

**Brand rules (hard):**
- Hanzo is a full AI SDK / AI cloud — never an "LLM gateway", never positioned
  against LiteLLM.
- Zen models are our own family; never reference upstream model names.
- Routes are `/v1/...` (never `/api/`). Base URL: `https://api.hanzo.ai`.

**Install:** Gradle `implementation("ai.hanzo:sdk:8.0.0")`. Maven Central
publication is pending; JitPack (`com.github.hanzo-kt:sdk:v8.0.0`) resolves the
repo directly today.

**Two SDK lines:** this is the generated Full Cloud SDK. The AI + agents flagship
is a separate line (Python `hanzo`, Rust `hanzo`, `@hanzo/ai`).

**Cross-links:** language org `hanzo-kt` · umbrella `hanzoai/sdk` · other
languages: Python (flagship) `hanzoai/python-sdk`, TypeScript `hanzo-js/sdk`,
Go `hanzo-go/sdk`, Rust `hanzo-rs/sdk`, C++ `hanzo-cpp/sdk`, Swift `hanzo-swift/sdk`
· [hanzo.ai](https://hanzo.ai) · [docs.hanzo.ai](https://docs.hanzo.ai).

Architecture spec: `~/work/hanzo/SDK-ARCHITECTURE.md`.
