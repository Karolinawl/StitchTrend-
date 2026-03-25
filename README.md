## Project Insights

StitchTrend is a capstone project created as part of the Data Analytics with Artificial Intelligence course.
The aim of this project is to explore how yarn weight and gauge relate to the popularity of knitting patterns on Ravelry, using data analysis tools learned during the course.

## Dataset Content

The dataset was collected from the Ravelry API and includes publicly available information about knitting and crochet patterns.

Planned data fields include:

-pattern name and category (e.g. hats, scarves, jumpers),

-craft type (knitting),

-yarn thickness (e.g. DK, worsted, bulky, 2ply, 4ply),

-gauge information (if available),

-free or paid status,

-popularity indicators such as number of projects,

The dataset size will be limited to what is needed for analysis and stored in versioned folders.

## Data Collection

Data is collected using the public, read-only Ravelry API.
API responses are initially stored in raw JSON format to preserve the original data structure.
Raw data is saved in versioned folders and later processed into a structured dataset suitable for analysis.
Data were collected in two stages: pattern discovery and pattern detail enrichment.

## Business Requirements

The project focus on:

-understanding which yarn thickness are linked to more popular patterns,

-comparing popularity between free and paid patterns,

-exploring whether gauge (stitch density) has any relationship with popularity,

-helping crafters and small handmade sellers decide what to make using yarn they already have,

-explore whether pattern popularity shows seasonal trends based on publication dates and pattern characteristics.

## Hypothesis and How to Validate

The following hypotheses were explored:

-Free patterns may be more popular than paid ones,

-Some yarn thickness may be more popular than others,

-Simpler or faster projects (using thicker yarn or lower stitch density) may attract more engagement,

-Patterns published in autumn and winter months show higher popularity than those published in spring and summer,

-Lightweight yarns (lace, fingering, sport) are more common in patterns published in spring and summer. 

-Heavier yarns (worsted, bulky) are more common in autumn and winter patterns.

These hypotheses will be explored using descriptive statistics, visualisations, and simple statistical tests where possible.

## Project Planning

A project board was used to organise and track progress.
https://github.com/users/Karolinawl/projects/3/views/1?template_dialog_tab=featured&layout_template=board

## Project Implementation

The project followed these steps:

1. Collect data from the Ravelry API.

2. Clean and prepare the dataset.

3. Explore the data using basic statistics and charts.

4. Test hypotheses using appropriate statistical methods.

5. Experiment with simple machine learning techniques.

6. Summarise findings and limitations.

Data will be managed using separate folders for raw, processed, and analysed data.

## Mapping Business Requirements to Data Visualisations

Each business requirement is supported by specific visualisations used in the analysis:

**1. Understanding which yarn thickness is linked to more popular patterns**  
→ Bar charts showing average popularity (projects_count / favourites_count) by yarn weight  

**2. Comparing popularity between free and paid patterns**  
→ Boxplots comparing distribution of popularity metrics for free vs paid patterns  

**3. Exploring the relationship between gauge and popularity**  
→ Scatter plots showing gauge values against popularity metrics  

**4. Identifying trends in pattern popularity**  
→ Histograms showing the distribution of popularity across patterns  

**5. Supporting crafters and small sellers in decision-making**  
→ Combined visual insights from multiple charts highlighting popular categories and trends  

Each visualisation directly supports a specific business question and helps translate data insights into practical understanding.

## Analysis Techniques Used

The project used:

-basic descriptive statistics (mean, median, standard deviation),

-exploratory data analysis (EDA),

-simple statistical tests,

The analysis may be limited by missing or inconsistent data, especially for gauge information.
Alternative approaches may be considered if some fields are unavailable.

## Dashboard (Power BI)

A simple interactive dashboard was created in Power BI to complement the exploratory data analysis.

The dashboard includes:
- yarn weight vs pattern popularity,
- comparison of free vs paid patterns,
- price vs popularity,
- overall distribution of pattern popularity.

The Power BI dashboard is included in the `dashboard/` folder as a .pbix file.
A PDF version is also provided for reference.

## Practical Value of the Analysis

This project provides insights into knitting and crochet pattern popularity using real-world data from the Ravelry platform.

The findings may be useful for:

- pattern designers looking to create more popular designs  
- crafters deciding what to make based on trends  
- small handmade sellers selecting products aligned with demand  

The analysis highlights trends in user engagement and supports better understanding of what drives popularity within the crafting community.

## Use of Generative AI Tools

ChatGPT and GitHub Copilot (within VS Code) were used only as a support during development, mainly to help with understanding code, debugging errors, and suggesting possible improvements.

All data analysis decisions, code implementation, and interpretation of results were completed independently by the author.

## Ethical Considerations

Only public data will be used

No personal or private user information will be collected

API credentials are stored in a .env file and loaded using python-dotenv to prevent accidental exposure of sensitive information in the codebase.

Any potential bias or data limitations will be acknowledged

## Unfixed Bugs

Some issues may remain unresolved, such as:

missing or unclear gauge values

incomplete yarn weight information

These issues are expected due to limitations of the source data.

## Development Roadmap

Future improvements may include:

better handling of gauge data

more advanced pattern matching

larger datasets

improved visualisations and models

## Deployment

The project may be run locally.
Deployment to a cloud platform will be considered if time allows.

## Main Data Analysis Libraries

Planned libraries include:

-pandas

-numpy

-scikit-learn

-matplotlib / plotly

## Credits

Data source: Ravelry API

Learning materials: Data Analytics with Artificial Intelligence course

## Acknowledgements

Thanks to course instructors, mentors, and peers for support during the learning process.

## Glossary

**Gauge**  
Gauge refers to the number of stitches and rows per unit of measurement (usually 10 cm / 4 inches). It determines how tight or loose a knitted or crocheted fabric is.

**Swatch (Gauge Sample)**  
A swatch is a small sample piece created to measure gauge. It helps ensure that the final project will have the correct size and fit.

**Yarn Weight**  
Yarn weight describes the thickness of the yarn (e.g. lace, fingering, DK, worsted, bulky). It affects the texture, drape, and speed of a project.

**Pattern Popularity**  
In this project, popularity is measured using indicators such as the number of projects and number of favourites on the Ravelry platform.
