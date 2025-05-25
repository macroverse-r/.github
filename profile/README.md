# macroverse

> A modern, modular ecosystem for international economic and social data analysis in R

## ⚠️ Work in Progress

**This ecosystem is currently under active development and should be considered experimental. Expect frequent changes, potential bugs, and breaking changes in the API. Use at your own risk for production work.**

- 🚧 **Active Development**: Core functionality is being implemented and tested
- 🔄 **Breaking Changes**: APIs may change without notice during development
- 🐛 **Known Issues**: Documentation may be incomplete and bugs are expected
- 📋 **Feedback Welcome**: Please report issues and suggestions

## Overview

The **macroverse** is a collection of R packages designed for seamless analysis of global economic and social panel data. Following the tidyverse model, macroverse provides specialized packages that work together while remaining independent and focused.

## 📦 Package Ecosystem

### Core Packages

| Package | Description | Status |
|---------|-------------|--------|
| **[macroverse](https://github.com/macroverse-r/macroverse)** | Meta-package that loads the entire ecosystem | 🚧 In Development |
| **[macrodata](https://github.com/macroverse-r/macrodata)** | Access to international economic and social data | 🚧 In Development |
| **[pplot](https://github.com/macroverse-r/pplot)** | Panel data visualization tools | 🚧 In Development |
| **[isomapper](https://github.com/macroverse-r/isomapper)** | ISO codes and country mapping utilities | 🚧 In Development |

### Utility Packages

| Package | Description | Status |
|---------|-------------|--------|
| **[mvcommon](https://github.com/macroverse-r/mvcommon)** | Shared utilities and validation functions | 🚧 In Development |
| **[mvlazy](https://github.com/macroverse-r/mvlazy)** | Quick analysis templates and convenience functions | 🚧 In Development |

## 🚀 Quick Start

### Install the Complete Ecosystem

```r
# ⚠️ Warning: Experimental packages - expect bugs and breaking changes
# Install the entire macroverse
devtools::install_github("macroverse-r/macroverse")
library(macroverse)

# Get help and overview
mv_help()
```

### Install Individual Packages

```r
# ⚠️ Warning: Individual packages are also experimental
# Install only what you need
devtools::install_github("macroverse-r/macrodata")
devtools::install_github("macroverse-r/pplot")
```

## 💡 Example Usage

### Load and Visualize Economic Data

```r
library(macroverse)

# Load GDP data for G7 countries
data <- md_data(
  ISO = "G7",
  formula = "GDP_C",
  years = c(2010, 2023)
)

# Create visualization
pp_plot_series(data, title = "G7 GDP Trends")
```

### Quick Economic Analysis

```r
# Balance of payments analysis
ml_quick("USA", c(2010, 2023), graph = "bop")

# Trade analysis with custom theme
ml_quick(c("CHN", "DEU", "JPN"), c(2015, 2023), 
         graph = "trade",
         theme = list(normalization = "GDP"))
```

### ISO Code Mapping

```r
# Convert country names to ISO codes
im_ctry2iso(c("United States", "Germany", "Japan"))
#> [1] "USA" "DEU" "JPN"

# Get country groups
eu_countries <- im_get_category("EU")
brics <- im_get_category("BRICS")
```

## 📊 Data Sources

The macroverse integrates data from major international organizations:

- **World Bank** (Development Indicators)
- **International Monetary Fund** (IFS, Balance of Payments)
- **Bank for International Settlements** (Credit, Banking)
- **OECD** (Main Economic Indicators)
- **Academic Sources** (Jordà-Schularick-Taylor, KOF, EM-DAT, etc.)

## 🎯 Key Features

- **🔗 Modular Design**: Use packages independently or together
- **📈 Rich Visualizations**: Publication-ready plots with minimal code
- **🌍 Global Coverage**: 200+ countries and territories
- **⏱️ Time Series**: Quarterly and yearly data from 1960s onwards
- **🎨 Quick Templates**: Pre-configured analysis workflows
- **🗺️ ISO Standards**: Comprehensive country code mapping
- **📚 Extensive Documentation**: Comprehensive guides and examples

## 📖 Documentation

- **[Getting Started Guide](https://macroverse-r.github.io/macroverse/)**
- **[Data Reference](https://macroverse-r.github.io/macrodata/)**
- **[Visualization Gallery](https://macroverse-r.github.io/pplot/)**
- **[Package Documentation](https://macroverse-r.github.io/)**

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Setup

```bash
# Clone the ecosystem
git clone https://github.com/macroverse-r/macroverse.git
cd macroverse

# Install development dependencies
Rscript -e "devtools::install_deps(dependencies = TRUE)"
```

## 📄 License

The macroverse ecosystem uses a **dual licensing model**:

- **🎓 Open Source**: [AGPL-3.0](LICENSE.md) for academic and non-commercial use
- **💼 Commercial**: Alternative licensing available for commercial applications

For commercial licensing inquiries, please contact the maintainer.

## 🛠️ Ecosystem Evolution

The macroverse represents a complete refactoring of the original [WPD (World Panel Data)](https://github.com/benjaminpeeters/wpd) package, following modern R package development best practices and the tidyverse model.

### Migration from WPD

If you're migrating from the WPD package:

```r
# Old WPD syntax
wp_data(ISO = "USA", formula = "GDP_C", years = c(2020, 2023))
wp_plot_series(data)

# New macroverse syntax
md_data(ISO = "USA", formula = "GDP_C", years = c(2020, 2023))
pp_plot_series(data)
```

## 👨‍💼 Maintainer

**Benjamin Peeters**  
Postdoctoral Researcher, PIK (Potsdam Institute for Climate Impact Research)  
📧 Contact: [benjaminpeeters@protonmail.com](mailto:benjaminpeeters@protonmail.com)  
🌐 Website: [benjaminpeeters.com](https://benjaminpeeters.com)

---

<div align="center">

**[⭐ Star us on GitHub](https://github.com/macroverse-r/macroverse)** | **[📚 Read the Docs](https://macroverse-r.github.io/)** | **[💬 Join Discussions](https://github.com/macroverse-r/macroverse/discussions)**

</div>