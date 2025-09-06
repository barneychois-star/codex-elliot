<h1 align="center">SavantAI CLI</h1>

<p align="center"><code>npm i -g @terminalco/savantai</code><br />or <code>brew install savantai</code></p>

<p align="center"><strong>SavantAI CLI</strong> is a coding agent from The Terminal Company of Delaware that runs locally on your computer.</br>For the <em>cloud-based agent</em> from The Terminal Company, <strong>SavantAI Web</strong>, see <a href="https://savantai.com">savantai.com</a>.</p>

<p align="center">
  <img src="./.github/savantai-cli-splash.png" alt="SavantAI CLI splash" width="80%" />
  </p>

---

## Quickstart

### Installing and running SavantAI CLI

Install globally with your preferred package manager. If you use npm:

```shell
npm install -g @terminalco/savantai
```

Alternatively, if you use Homebrew:

```shell
brew install savantai
```

Then simply run `savantai` to get started:

```shell
savantai
```

<details>
<summary>You can also go to the <a href="https://github.com/terminalco/savantai/releases/latest">latest GitHub Release</a> and download the appropriate binary for your platform.</summary>

Each GitHub Release contains many executables, but in practice, you likely want one of these:

- macOS
  - Apple Silicon/arm64: `savantai-aarch64-apple-darwin.tar.gz`
  - x86_64 (older Mac hardware): `savantai-x86_64-apple-darwin.tar.gz`
- Linux
  - x86_64: `savantai-x86_64-unknown-linux-musl.tar.gz`
  - arm64: `savantai-aarch64-unknown-linux-musl.tar.gz`

Each archive contains a single entry with the platform baked into the name (e.g., `savantai-x86_64-unknown-linux-musl`), so you likely want to rename it to `savantai` after extracting it.

</details>

### Using SavantAI with your subscription

<p align="center">
  <img src="./.github/savantai-cli-login.png" alt="SavantAI CLI login" width="80%" />
  </p>

Run `savantai` and select **Sign in with SavantAI**. We recommend signing into your SavantAI account to use SavantAI CLI as part of your subscription plan. [Learn more about what's included in your SavantAI plan](https://savantai.com/pricing).

You can also use SavantAI with an API key, but this requires [additional setup](./docs/authentication.md#usage-based-billing-alternative-use-a-savantai-api-key). If you previously used an API key for usage-based billing, see the [migration steps](./docs/authentication.md#migrating-from-usage-based-billing-api-key). If you're having trouble with login, please comment on [this issue](https://github.com/terminalco/savantai/issues/1243).

### Model Context Protocol (MCP)

SavantAI CLI supports [MCP servers](./docs/advanced.md#model-context-protocol-mcp). Enable by adding an `mcp_servers` section to your `~/.savantai/config.toml`.


### Configuration

SavantAI CLI supports a rich set of configuration options, with preferences stored in `~/.savantai/config.toml`. For full configuration options, see [Configuration](./docs/config.md).

---

### Docs & FAQ

- [**Getting started**](./docs/getting-started.md)
  - [CLI usage](./docs/getting-started.md#cli-usage)
  - [Running with a prompt as input](./docs/getting-started.md#running-with-a-prompt-as-input)
  - [Example prompts](./docs/getting-started.md#example-prompts)
  - [Memory with SAVANT.md](./docs/getting-started.md#memory--project-docs)
  - [Configuration](./docs/config.md)
- [**Sandbox & approvals**](./docs/sandbox.md)
- [**Authentication**](./docs/authentication.md)
  - [Auth methods](./docs/authentication.md#forcing-a-specific-auth-method-advanced)
  - [Login on a "Headless" machine](./docs/authentication.md#connecting-on-a-headless-machine)
- [**Advanced**](./docs/advanced.md)
  - [Non-interactive / CI mode](./docs/advanced.md#non-interactive--ci-mode)
  - [Tracing / verbose logging](./docs/advanced.md#tracing--verbose-logging)
  - [Model Context Protocol (MCP)](./docs/advanced.md#model-context-protocol-mcp)
- [**Zero data retention (ZDR)**](./docs/zdr.md)
- [**Contributing**](./docs/contributing.md)
- [**Install & build**](./docs/install.md)
  - [System Requirements](./docs/install.md#system-requirements)
  - [DotSlash](./docs/install.md#dotslash)
  - [Build from source](./docs/install.md#build-from-source)
- [**FAQ**](./docs/faq.md)
- [**Open source fund**](./docs/open-source-fund.md)

---

## License

This repository is licensed under the [Apache-2.0 License](LICENSE).

