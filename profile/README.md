<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nexa-Language/.github/main/profile/assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Nexa-Language/.github/main/profile/assets/banner-light.svg">
  <img alt="Nexa — An agent-native language and runtime. Define the work. Make execution explicit." src="https://raw.githubusercontent.com/Nexa-Language/.github/main/profile/assets/banner-light.svg" width="1200">
</picture>

### An agent-native language and runtime.

Nexa gives people and models a shared language for building agents. Define tools, contracts, and control flow in `.nx`; let the runtime manage model protocols, execution budgets, approvals, and recoverable state.

**[Start with Nexa](https://github.com/Nexa-Language/Nexa#readme)** · **[Documentation](https://docs.nexa-lang.com/en/quickstart/)** · **[中文文档](https://docs.nexa-lang.com/quickstart/)** · [Website](https://www.nexa-lang.com)

---

#### Write the workflow. Keep the execution visible.

```nexa
agent Analyst {
    prompt: "Analyze the evidence and explain your conclusions."
    model: "openai/gpt-5.4-mini"
    provider_api: "responses"
    timeout: 120
    max_tool_calls: 4
}

flow main {
    findings = Analyst.run("Explain the trade-offs of checkpointing.");
    print(findings);
}
```

Save this as `analysis.nx`, configure the OpenAI provider, then run `nexa run analysis.nx`. Follow the [installation and configuration guide](https://docs.nexa-lang.com/en/quickstart/) for the supported toolchain and credentials.

Python is the reference compiler and runtime. The Rust AVM develops a defined execution subset, checked against shared conformance cases. See the [implementation and support boundaries](https://github.com/Nexa-Language/Nexa#readme) for the current release.

#### One language. A working toolchain.

| Project | Start here |
| :--- | :--- |
| **[Nexa](https://github.com/Nexa-Language/Nexa)** | Language, compiler, runtime, CLI, and executable examples. |
| **[Nexa Code](https://github.com/Nexa-Language/Nexa-Code)** | A coding agent built in Nexa, with a terminal interface for tasks and tools. |
| **[VS Code extension](https://github.com/Nexa-Language/Nexa-extension)** | Language support and development tools for `.nx` programs. |
| **[Documentation](https://github.com/Nexa-Language/Nexa-docs)** | Guides, language reference, runtime contracts, and migration notes. |

#### Research, in the open.

Explore the projects alongside the language: [Skill-Compiler](https://github.com/Nexa-Language/Skill-Compiler), [SLIM-ARC](https://github.com/Nexa-Language/SLIM-ARC), [RAMP](https://github.com/Nexa-Language/RAMP), [EpiContext](https://github.com/Nexa-Language/EpiContext), [Nexa-net](https://github.com/Nexa-Language/Nexa-net), and [V-Core](https://github.com/Nexa-Language/V-Core). Each repository documents its own scope, evidence, and development status.

---

**Build with us.** Start with a [small example](https://github.com/Nexa-Language/Nexa/tree/main/examples), [report an issue](https://github.com/Nexa-Language/Nexa/issues), or read the [contribution guide](https://github.com/Nexa-Language/.github/blob/main/CONTRIBUTING.md).
