# Post45 Data Collective Website

https://data.post45.org/

This is the website for the Post45 Data Collective, which uses [Quarto](https://quarto.org/), the [R DT library](https://rstudio.github.io/DT/), and the [JavaScript Tabulator library](https://tabulator.info/).

Benefits of Quarto include: publication-quality, citeable articles and references that can be recognized by Google Scholar; easy integration with code such as data tables; articles that are created with Markdown, which can ease the publication pipeline by preserving formatting and links from submitted Word Documents and Google Docs; entirely free and open-source tools.

## Setup

### Prerequisites

1. **Install R** (version 4.3 or higher recommended)

   - Download from [CRAN](https://cran.r-project.org/)

2. **Install Quarto**

   - Download from [quarto.org](https://quarto.org/docs/get-started/)

3. **Install a code editor** (optional but recommended)
   - **RStudio**: Download from [posit.co](https://posit.co/download/rstudio-desktop/)
   - **VS Code**: Download from [code.visualstudio.com](https://code.visualstudio.com/)
     - Install the [Quarto extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto) for VS Code

### Installation

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/Post45-Website-Quarto.git
cd website
```

2. **Install R packages:**

Open R or RStudio and run:

```r
# Install renv if you don't have it
install.packages("renv")

# Restore all required R packages (including dplyr, knitr, rmarkdown, etc.)
renv::restore()
```

If using the command line, type `R` to open the R console, run the commands above, then type `q()` to quit R.

This will install all the R packages specified in `renv.lock`, ensuring you have the exact same dependencies as the project requires.

### Running the Site

To preview the website locally:

**Option 1: Command line**

```bash
quarto preview
```

**Option 2: VS Code**

- Open a `.qmd` file and click the "Preview" button in the top right corner of the editor

To render the site:

```bash
quarto render
```
