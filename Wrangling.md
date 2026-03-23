# Issues encountered
<p align="justify">
The raw dataset downloaded from the CIHI Your Health System Indicator Library was significantly large, containing approximately 48,002 rows and over 100 health system indicators spanning multiple domains. Due to the size of the file, opening and working with the data proved challenging, the Excel files crashed repeatedly during initial attempts to explore and load the data, making direct manipulation of the full dataset impractical.

# How addressed each issue
<p align="justify">
To resolve the file size and performance issue, the scope of the dataset was intentionally narrowed to focus only on mental health-related indicators. The full indicator list was reviewed, and four indicators directly relevant to mental health were identified: Canadians With a Mental Health Disorder Who Have an Unmet Need for Mental Health Care, Self-Harm Hospitalizations, Self-Harm Including Suicide, and Wait Times for Community Mental Health Counselling. This filtering reduced the dataset from 48,002 rows to 616 rows, making it stable and manageable to work with. The filtered dataset was then exported into a Tableau Hyper extract dataset3.hyper to enable efficient loading and visualization in Tableau without further performance issues.

# Assumptions and decisions made during cleaning
<p align="justify">
Two key decisions were made during the wrangling process. First, since both downloaded Excel files contained identical data, only File 1 was used as the primary source for filtering and export; File 2 was retained solely for verification purposes. Second, indicators that combined mental health and substance use outcomes, such as repeat hospital stays and emergency room visits for mental health and substance use, were reviewed for any sub-category breakdowns that might isolate mental health alone. Finding none, these indicators were excluded entirely rather than included with the risk of misrepresenting the analysis as purely mental health focused.
</p>