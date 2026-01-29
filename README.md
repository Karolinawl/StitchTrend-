## Project Insights

StitchTrend is a capstone project created as part of the Data Analytics with Artificial Intelligence course.
The aim of this project is to explore how yarn weight and gauge relate to the popularity of knitting patterns on Ravelry, using data analysis tools learned during the course.

## Dataset Content

The dataset will be collected from the Ravelry API and will include publicly available information about knitting and crochet patterns.

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

The project will focus on:

-understanding which yarn thickness are linked to more popular patterns,

-comparing popularity between free and paid patterns,

-exploring whether gauge (stitch density) has any relationship with popularity,

-helping crafters and small handmade sellers decide what to make using yarn they already have,

-explore whether pattern popularity shows seasonal trends based on publication dates and pattern characteristics.

## Hypothesis and How to Validate

Planned hypotheses include:

-Free patterns may be more popular than paid ones,

-Some yarn thickness may be more popular than others,

-Simpler or faster projects (using thicker yarn or lower stitch density) may attract more engagement,

-Patterns published in autumn and winter months show higher popularity than those published in spring and summer,

-Lightweight yarns (lace, fingering, sport) are more common in patterns published in spring and summer. 

-Heavier yarns (worsted, bulky) are more common in autumn and winter patterns.

These hypotheses will be explored using descriptive statistics, visualisations, and simple statistical tests where possible.

## Project Plan

Planned steps for the project:

1. Collect data from the Ravelry API.

2. Clean and prepare the dataset.

3. Explore the data using basic statistics and charts.

4. Test hypotheses using appropriate statistical methods.

5. Experiment with simple machine learning techniques.

6. Summarise findings and limitations.

Data will be managed using separate folders for raw, processed, and analysed data.

## Mapping Business Requirements to Data Visualisations

Planned visualisations include:

-bar charts showing yarn weight and popularity,

-boxplots comparing free and paid patterns,

-scatter plots for price and popularity,

-histograms showing the distribution of popularity,

Each visualisation will be used to support a specific business question.

## Analysis Techniques Used

The project will use:

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

Due to limited access to Power BI after the course, the dashboard was exported as a PDF file, it's available as PDF file in the project folder.

## Use of Generative AI Tools

ChatGPT and GitHub Copilot (within VS Code) were used only as a support during development, mainly to help with understanding code, debugging errors, and suggesting possible improvements.

All data analysis decisions, code implementation, and interpretation of results were completed independently by the author.

## Ethical Considerations

Only public data will be used

No personal or private user information will be collected

API credentials are stored in a .env file and loaded using python-dotenv to prevent accidental exposure of sensitive information in the codebase.

Any potential bias or data limitations will be acknowledged

## Dashboard Design

If time allows, a dashboard will be created to present key insights in a clear and simple way.

Planned dashboard elements include:

summary metrics

charts showing yarn thicknes and popularity

simple filtering options

a basic gauge-to-yarn-weight helper

The dashboard will be designed for both technical and non-technical users.

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
