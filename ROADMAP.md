# Mnemex Roadmap

This document outlines the development roadmap for Mnemex. For detailed implementation notes, see [future_roadmap.md](future_roadmap.md).

## Version 0.5.5 (Released ✅ - 2025-10-30)

**Status:** Latest stable release with major UX improvements

### 🎉 Highlights
- ✅ **Automatic LTM index management** - Major UX improvement
  - `promote_memory` auto-updates LTM index after promotion
  - `search_unified` auto-rebuilds stale/missing indexes
  - **No more manual `mnemex-index-ltm` needed**
  - Newly promoted memories immediately searchable
- ✅ **README refactored** - Eliminated repetition, improved flow
- ✅ **Logo added** - Brand identity established

## Version 0.5.0 (Released ✅ - 2025-10-18)

**Status:** Stable baseline with expanded test coverage

### 🛡️ Security & Testing
- ✅ 4 new security test modules (100+ tests)
- ✅ 3000+ new tests added (decay, LTM, search, storage)
- ✅ Bandit, CodeQL, and SBOM generation in CI
- ✅ Secrets detection and input validation
- ✅ Repository cleanup (25+ stale branches removed)

## Version 1.0.0 (Released ✅ - 2025-10-09)

**Status:** Production-ready, feature-complete

- ✅ 11 MCP tools for memory management
- ✅ Temporal decay with 3 models (power-law, exponential, two-component)
- ✅ JSONL storage with in-memory indexing
- ✅ Algorithmic memory consolidation
- ✅ Unified search across STM and LTM
- ✅ Git integration for backups
- ✅ Obsidian vault integration
- ✅ 7 CLI commands
- ✅ Complete documentation suite
- ✅ CI/CD with GitHub Actions

## Version 1.1.0 (Planned - Q1 2026)

**Focus:** Stability, Testing, Security

### High Priority

- [x] **Security Hardening** ([#6](https://github.com/simplemindedbot/mnemex/issues/6)) ⏳ ~85% Complete
  - ✅ Dependency scanning (Dependabot, pip-audit)
  - ✅ Code security scanning (Bandit, CodeQL)
  - ✅ Supply chain verification (SBOM generation)
  - ✅ SECURITY.md policy
  - ✅ Input validation and path traversal prevention
  - ✅ Secrets detection (100+ security tests added)

- [x] **Fix mypy Type Checking** ([#1](https://github.com/simplemindedbot/mnemex/issues/1)) ✅ COMPLETED (v0.4.0)
  - ✅ Fixed 30+ type errors
  - ✅ Re-enabled mypy in CI
  - ✅ Added pre-commit hooks

- [x] **Improve Test Coverage** ([#7](https://github.com/simplemindedbot/mnemex/issues/7)) ⏳ ~65% Complete
  - Target: 80%+ coverage
  - ✅ 3000+ new tests added (415 decay, 797 LTM, 1159 search, 921 storage)
  - ✅ 4 comprehensive security test modules
  - ✅ Core module coverage significantly improved
  - ⏳ CLI tool tests (remaining)
  - ⏳ Integration tests (remaining)

- [ ] **Production Hardening** ([#8](https://github.com/simplemindedbot/mnemex/issues/8)) ⏳ ~20% Complete
  - ✅ Auto LTM index management (v0.5.5 - eliminates manual rebuilding)
  - ⏳ File corruption handling (partial)
  - ⏳ Configuration validation (partial)
  - ⏳ Graceful degradation (remaining)
  - ⏳ File locking for concurrent access (remaining)
  - ⏳ Better logging with rotation (remaining)

### Medium Priority

- [ ] **Platform Testing** ([#9](https://github.com/simplemindedbot/mnemex/issues/9))
  - Windows testing (community help needed)
  - Linux testing (community help needed)
  - Cross-platform bug fixes

- [ ] **Performance Optimizations** ([#4](https://github.com/simplemindedbot/mnemex/issues/4)) ⏳ ~30% Complete
  - ✅ Performance optimization infrastructure added
  - ✅ Auto LTM index management (major performance win)
  - ⏳ Benchmark suite (remaining)
  - ⏳ Tag/entity indexing (remaining)
  - ⏳ Embedding cache (remaining)
  - ⏳ Score caching (remaining)

## Version 1.2.0 (Planned - Q2 2026)

**Focus:** Advanced Features, User Experience

### High Priority

- [x] **Spaced Repetition** ([#2](https://github.com/simplemindedbot/mnemex/issues/2)) ✅ COMPLETED (v0.5.1)
  - ✅ Conversation-based spaced repetition system
  - ✅ Natural reinforcement through cross-domain usage detection
  - ✅ Alternative implementation to explicit flashcard-style reviews

- [ ] **Adaptive Decay Parameters** ([#3](https://github.com/simplemindedbot/mnemex/issues/3))
  - Category-based decay profiles
  - Usage-pattern learning
  - Auto-detection from tags/content

### Low Priority

- [x] **LLM-Assisted Consolidation** ([#5](https://github.com/simplemindedbot/mnemex/issues/5)) ✅ COMPLETED (v1.0.0)
  - ✅ Algorithmic consolidation production-ready with 100% test coverage
  - ✅ Preview/apply modes for safe consolidation
  - ✅ LLM assistance deemed unnecessary for current use cases

## Version 2.0.0 (Future)

**Focus:** Advanced AI Features, Ecosystem Integration

- Machine learning for decay parameter optimization
- Multi-user support
- API server mode
- Plugins/extensions system
- Integration with popular tools (Raycast, Alfred, etc.)
- Mobile client support (iOS, Android)

---

## Contributing

We welcome contributions! Priority areas:

1. **Platform Testing** - Help test on Windows/Linux ([#9](https://github.com/simplemindedbot/mnemex/issues/9))
2. **Security** - Implement security hardening ([#6](https://github.com/simplemindedbot/mnemex/issues/6))
3. **Testing** - Increase coverage ([#7](https://github.com/simplemindedbot/mnemex/issues/7))

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## Links

- [GitHub Issues](https://github.com/simplemindedbot/mnemex/issues)
- [Detailed Roadmap](future_roadmap.md)
- [Documentation](docs/)
- [Contributing Guide](CONTRIBUTING.md)

---

**Last Updated:** 2025-10-31
**Current Version:** 0.5.5
**Next Release:** 0.6.0 (Q1 2026 - Production Hardening & Platform Testing)
