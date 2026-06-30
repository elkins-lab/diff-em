# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.2] - 2026-06-30

### Added
- Added interactive Cryo-EM fitting tutorial (`examples/interactive_tutorials/cryo_em_fitting_tutorial.ipynb`).
- Added tests to cover edge cases for `simulate_density` and `cross_correlation` (e.g., flat maps, orthogonal maps).
- Integrated `mkdocs-jupyter` to render tutorial notebooks on the documentation site.

### Changed
- Restructured tutorials into `examples/interactive_tutorials/` and updated README with Google Colab links.
- Simplified package installation instructions in documentation.
- Updated CI workflow to use `pre-commit run --all-files` instead of raw checks.

### Fixed
- Fixed GitHub Actions `mypy` syntax error with NumPy 2.x type stubs by resolving through the pinned `pre-commit` environment.
- Fixed `Node.js` deprecation warnings in CI by forcing JavaScript actions to use Node.js 24.
- Added input validation for edge cases in `simulate_density` and `cross_correlation` (e.g., non-positive sigma, mismatched map shapes).

## [0.1.1] - 2026-06-07

### Security
- Removed compromised `polyfill.io` CDN script from MkDocs configuration to resolve supply-chain vulnerability.
