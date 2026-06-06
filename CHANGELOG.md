# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Fixed
- `ProviderInitError`-Absturz bei OpenCode CLI 1.16.2 + `@ai-sdk/fireworks` < 2.0.53
- `opencode-config-install.sh` führt jetzt automatisch `npm install @ai-sdk/fireworks@latest @ai-sdk/openai-compatible@latest` aus
- Alte Sessions liefen noch im RAM, neue crashten bei SDK-Neuinitialisierung

### Added
- Initial SIN-Code-Bundle integration (ceo-audit workflow v3)
- OpenCode MCP server registration under `OpenSIN-Code/SIN-Code-FireworksAI-OpenCode-Config`
- Repository-level `SIN_GITHUB_FALLBACK_TOKEN` secret for the App commenter fallback
- Fireworks AI pool config for OpenCode CLI: 12 models at temperature 0
- Base URL `https://sinatorpool-router.delqhi.com/inference/v1` with auto-failover
- One-line install via `opencode-config-install.sh` / `opencode-config-repair.sh`
- `config.example.json`, `INSTALL.md`, `requirements.txt`, and `tests/` for validation

### Security
- All commits verified via `git-immortal-commit` (annotated tags)
- No real API keys committed — `config.example.json` ships with placeholders only
