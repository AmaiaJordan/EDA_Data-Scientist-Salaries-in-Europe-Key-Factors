
# Labor Market for Data Scientists in Europe: What Factors Influence Salary?

## Project Overview
This project explores salary patterns for data scientists across Europe, focusing on factors that impact compensation. Using data from 2020 to 2024, it aims to uncover insights into how variables like experience level, job category, location, and company size affect salaries in this high-demand field.

## Objectives
- Identify key patterns and characteristics affecting data scientist salaries in Europe.
- Analyze variable influences on total earnings for professionals in the data science field.
- Provide insights for both candidates and employers to make informed decisions in a competitive job market.

## Dataset Description
The data used in this project is sourced from the **Data Science Salaries Dataset** on Kaggle. The dataset comprises 14,838 rows and 11 columns, covering data collected between 2020 and 2024.

### Key Variables
| Variable                  | Description                                                                 | Type               |
|---------------------------|-----------------------------------------------------------------------------|--------------------|
| `work_year`               | Year of salary data collection                                             | Year               |
| `experience_level`        | Experience level of the employee (Junior, Mid-level, Senior, Expert)       | Ordinal Categorical|
| `employment_type`         | Type of employment (Full-Time, Part-Time, Contract)                        | Ordinal Categorical|
| `job_title`               | Role of the employee (e.g., Data Analyst, Data Scientist)                  | Nominal Categorical|
| `salary`                  | Salary in specified currency                                               | Numeric            |
| `salary_currency`         | Currency used in salary                                                    | Nominal Categorical|
| `salary_in_usd`           | Salary converted to USD for standardization                                | Numeric            |
| `employee_residence`      | Employee's place of residence                                              | Nominal Categorical|
| `remote_ratio`            | Percentage of remote work allowed                                         | Ordinal Categorical|
| `company_location`        | Location of the hiring company                                             | Ordinal Categorical|
| `company_size`            | Company size (Small, Medium, Large)                                        | Ordinal Categorical|

### Additional Variables Created for Analysis
| Variable                  | Description                                                                                  | Type               |
|---------------------------|----------------------------------------------------------------------------------------------|--------------------|
| `job_category`            | Higher-level job categories (Data Analyst, Data Scientist, Data Architect/Engineer, Manager) | Nominal Categorical|
| `salary_in_euro`          | Salary converted to Euro                                                                     | Numeric            |
| `country_employee_residence`| Country name associated with ISO code                                                     | Ordinal Categorical|
| `europe_zone`             | Region within Europe based on employee residence                                             | Ordinal Categorical|
| `experience_level_num`    | Numeric conversion of experience level                                                       | Numeric            |
| `salary_category_num`     | Numeric conversion of salary categories                                                      | Numeric            |
| `salary_category`         | Salary grouped in ranges (e.g., ‘under 40,000€,’ ‘40,000€-50,000€’)                         | Ordinal Categorical|
| `company_size_num`        | Numeric conversion of company size categories                                                | Numeric            |

## Data Preprocessing
- **Data Quality**: No missing values or duplicates were found.
- **Data Type Conversion**: Not required, as data types were compatible with analysis requirements.
- **Filtering**: Focused on data scientists residing in Europe.

## Analysis Approach

### 1. Univariate Analysis
- **Distribution and Trends**: Each variable's distribution was examined to understand its relevance and distribution across values.
- **Central Tendency**: The `salary_in_euro` variable showed a general upward trend in average salary until 2023, with a slight decrease in 2024.
- **Observations**:
  - The United Kingdom is the leading location for data science professionals.
  - Remote work is less common than expected, with on-site work prevailing.
  - Most companies are medium-sized (80.58%), typically with 50-250 employees and revenue of 10M-50M Euros.

### 2. Bivariate and Multivariate Analysis
- Key influential variables:
  - **Employee Residence**: Professionals in Great Britain and Western Europe generally earn higher salaries.
  - **Job Category & Experience Level**: Higher roles (e.g., Data Architect/Engineer) and advanced experience levels correlate with higher salaries.
  - **Company Size**: Larger companies generally offer higher salaries.

### 3. Challenges
- **Categorical Variables**: Complexities in determining correlations due to categorical data types. Attempts to use radar charts for correlation visualization were not effective. Instead, histograms and bar charts provided clearer insights.
- **Variable Consolidation**: Grouped categories (e.g., `job_title` to `job_category`) to simplify analysis.

## Conclusions
This analysis provides a comprehensive look at factors impacting data science salaries across Europe. Key findings:
- **Experience and Role**: Advanced roles like Data Architect/Engineer command higher salaries, as do senior professionals.
- **Geographic Location**: Salaries are generally higher in the UK and Western Europe.
- **Company Size**: Medium and large companies tend to offer more competitive compensation.
  
For **data science professionals**, acquiring high-demand skills (e.g., AI, cloud computing) and considering relocation could enhance salary prospects. For **employers**, a competitive salary strategy should factor in local living costs, technical skill requirements, and investment in professional development.

## Usage
This dataset and analysis offer valuable insights for:
- Benchmarking salaries by experience, job title, and company size.
- Understanding the impact of remote work and geographic factors on compensation.
  
## License
This project is available under the MIT License.

---

Explore the dataset and uncover patterns in the European labor market for data scientists!
