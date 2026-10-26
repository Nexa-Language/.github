<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nexa-Language/.github/main/profile/assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Nexa-Language/.github/main/profile/assets/banner-light.svg">
  <img alt="Nexa — An agent-native language and runtime. Define the work. Make execution explicit." src="https://raw.githubusercontent.com/Nexa-Language/.github/main/profile/assets/banner-light.svg" width="1200">
</picture>

### An agent-native language and runtime.

Nexa 3.0 brings **Open Programs** to `.nx`: declare a goal, state its contract, and leave the implementation open. The runtime resolves that work inside a bounded environment, records the evidence, and keeps revisions and patch permissions explicit.

**[Start with Nexa](https://github.com/Nexa-Language/Nexa#readme)** · **[Documentation](https://docs.nexa-lang.com/en/quickstart/)** · **[中文文档](https://docs.nexa-lang.com/quickstart/)** · [Website](https://www.nexa-lang.com)

---

#### Define the result. Keep the evidence.

```nexa
language "3.0"
program Sum {
    goal total() -> Int {
        intent "Sum inputs.get('values', []). Return zero for an empty list."
        capabilities [sandbox.exec]
        ensure checks.sum
        implementation open
    }
}
```

Save this as `sum.nx` and run `nexa check sum.nx --json`. The check inspects the source and reports the open obligation without a model call or container. To resolve and run it, configure the provider, `checks.sum`, execution budget, and pinned OCI environment described in the [Open Programs guide](https://docs.nexa-lang.com/en/open_programs/) and [environment setup](https://docs.nexa-lang.com/en/open_environments/).

Inspect the [evidence](https://docs.nexa-lang.com/en/open_evidence/) behind each result. Preview a maintenance patch, then issue an [exact grant](https://docs.nexa-lang.com/en/open_grants/) before applying it. [Revisions and durable activities](https://docs.nexa-lang.com/en/open_revisions/) make interrupted work recoverable.

Python is the reference 3.0 compiler and runtime; Open Programs execution uses Linux or macOS with Docker/OCI. Existing unversioned 2.4 agent and flow programs remain supported. The Rust AVM covers a defined 2.4 subset. See the [3.0 migration guide](https://docs.nexa-lang.com/en/migration_30/) for the version boundary.

#### One language. A working toolchain.

| Project | Start here |
| :--- | :--- |
| **[Nexa](https://github.com/Nexa-Language/Nexa)** | Language, compiler, runtime, CLI, and executable examples. |
| **[Nexa Code](https://github.com/Nexa-Language/Nexa-Code)** | A terminal workspace for goals, evidence, reviewed patches, and existing agent workflows. |
| **[VS Code extension](https://github.com/Nexa-Language/Nexa-extension)** | Source checks, authoring, revisions, and runtime inspection inside the editor. |
| **[Documentation](https://github.com/Nexa-Language/Nexa-docs)** | Bilingual 3.0 guides, runtime contracts, and the 2.4 compatibility path. |

#### Research, in the open.

Explore the projects alongside the language: [Skill-Compiler](https://github.com/Nexa-Language/Skill-Compiler), [SLIM-ARC](https://github.com/Nexa-Language/SLIM-ARC), [RAMP](https://github.com/Nexa-Language/RAMP), [EpiContext](https://github.com/Nexa-Language/EpiContext), [Nexa-net](https://github.com/Nexa-Language/Nexa-net), and [V-Core](https://github.com/Nexa-Language/V-Core). Each repository documents its own scope, evidence, and development status.

---

**Build with us.** Start with a [small example](https://github.com/Nexa-Language/Nexa/tree/main/examples), [report an issue](https://github.com/Nexa-Language/Nexa/issues), or read the [contribution guide](https://github.com/Nexa-Language/.github/blob/main/CONTRIBUTING.md).
