# macroverse

A modular ecosystem for international economic and social data analysis in R.

## Status

This ecosystem is under active development and should be considered experimental. APIs may change without notice, documentation is incomplete in places, and bugs are expected. Use at your own risk for production work; feedback is welcome.

## Package ecosystem

Core packages:

| Package | Description |
|---------|-------------|
| [macroverse](https://github.com/macroverse-r/macroverse) | Meta-package that loads the entire ecosystem |
| [macrodata](https://github.com/macroverse-r/macrodata) | Access to international economic and social data |
| [pplot](https://github.com/macroverse-r/pplot) | Panel data visualization tools |
| [isomapper](https://github.com/macroverse-r/isomapper) | ISO codes and country mapping utilities |

Utility packages:

| Package | Description |
|---------|-------------|
| [mvcommon](https://github.com/macroverse-r/mvcommon) | Shared utilities and validation functions |
| [mvlazy](https://github.com/macroverse-r/mvlazy) | Quick analysis templates and convenience functions |

## Installation

```r
# Install the meta-package and its dependencies
devtools::install_github("macroverse-r/macroverse")
library(macroverse)
```

For per-package usage examples, see the README on each individual package's repo.

## Data sources

The macroverse integrates data from major international organizations:

- World Bank (Development Indicators)
- International Monetary Fund (IFS, Balance of Payments)
- Bank for International Settlements (Credit, Banking)
- OECD (Main Economic Indicators)
- Academic sources (Jordà-Schularick-Taylor, KOF, EM-DAT, etc.)

## Documentation

See each package's repo for installation, usage, and reference documentation. A unified pkgdown site is planned but not yet deployed.

## Contributing

See [CONTRIBUTING.md](https://github.com/macroverse-r/.github/blob/main/CONTRIBUTING.md) for the workflow, [PULL_REQUEST_TEMPLATE.md](https://github.com/macroverse-r/.github/blob/main/PULL_REQUEST_TEMPLATE.md) for PR conventions, [SUPPORT.md](https://github.com/macroverse-r/.github/blob/main/SUPPORT.md) for where to ask questions, and [CODE_OF_CONDUCT.md](https://github.com/macroverse-r/.github/blob/main/CODE_OF_CONDUCT.md) for community guidelines.

## License

The macroverse ecosystem uses a dual-licensing model: AGPL-3.0 for academic and non-commercial use; alternative licensing is available for commercial applications. For commercial licensing inquiries, see [SUPPORT.md](https://github.com/macroverse-r/.github/blob/main/SUPPORT.md).

## Maintainer

Benjamin Peeters
Postdoctoral Researcher, PIK (Potsdam Institute for Climate Impact Research)
Contact: benjaminpeeters@protonmail.com
Website: https://benjaminpeeters.com
