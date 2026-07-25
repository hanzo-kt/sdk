# Hanzo Kotlin SDK

**Hanzo Cloud SDK for Kotlin** — the full `/v1` cloud surface (AI, agents, compute,
data, network, security, platform, observe, web3, apps) as a coroutine-native
client for the JVM and Android. Generated from the [Hanzo OpenAPI spec](https://github.com/hanzoai/openapi), so it never drifts from the API.

## Install

Gradle (Kotlin DSL):

```kotlin
dependencies {
    implementation("ai.hanzo:sdk:8.0.0")
}
```

> Maven Central publication of `ai.hanzo:sdk` is in progress. Until it lands you
> can consume this repo directly via [JitPack](https://jitpack.io):
> add `maven("https://jitpack.io")` to your repositories and
> `implementation("com.github.hanzo-kt:sdk:v8.0.0")`.

## Quickstart

```kotlin
import ai.hanzo.sdk.apis.AgentsApi
import ai.hanzo.sdk.infrastructure.ApiClient
import kotlinx.coroutines.runBlocking

fun main() = runBlocking {
    // Base URL defaults to https://api.hanzo.ai. Authenticate with your Hanzo API key (Bearer).
    ApiClient.accessToken = System.getenv("HANZO_API_KEY")

    // Every service is an *Api class (AgentsApi, AiApi, NexusApi, ComputeApi, …), coroutine-native.
    val agents = AgentsApi().chatGetAgents()
    println(agents)
}
```

Every endpoint and model is documented under [`docs/`](./docs) and in
[`GENERATED.md`](./GENERATED.md) (the generator's full API index).

## Two SDK lines

- **Full Cloud SDK (this package)** — the entire `/v1` surface, generated from OpenAPI.
- **AI + agents** — the hand-crafted flagship library; see the sibling-language SDKs.

## Hanzo — the Open AI Cloud

Open source · every language · on-chain settlement.
[hanzo.ai](https://hanzo.ai) · [docs.hanzo.ai](https://docs.hanzo.ai)

**SDKs in every language** — [Python](https://github.com/hanzoai/python-sdk) (flagship) ·
[TypeScript](https://github.com/hanzo-js/sdk) ·
[Go](https://github.com/hanzo-go/sdk) ·
[Rust](https://github.com/hanzo-rs/sdk) ·
[C++](https://github.com/hanzo-cpp/sdk) ·
[Swift](https://github.com/hanzo-swift/sdk) ·
[Kotlin](https://github.com/hanzo-kt/sdk) ·
[umbrella](https://github.com/hanzoai/sdk)

## License

Apache-2.0.
