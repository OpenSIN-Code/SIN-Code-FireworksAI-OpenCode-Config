# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

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
