# Netflix Content Analysis Dashboard – Excel

## 📊 Project Overview

This project is an interactive **Netflix Content Analysis Dashboard** created using Microsoft Excel. The dashboard analyzes Netflix Movies and TV Shows based on content type, release year, country, genre, and rating.

The project demonstrates data cleaning, transformation, data modeling, DAX calculations, PivotTables, PivotCharts, and interactive slicers in Excel.

## 🛠️ Tools & Technologies

- Microsoft Excel
- Power Query
- Power Pivot
- DAX
- PivotTables
- PivotCharts
- Slicers
- Data Modeling

## 📂 Dataset

The project uses the Netflix Movies and TV Shows dataset from Kaggle.

Dataset: Shivam Bansal – Netflix Shows

## 🔄 Data Preparation

Power Query was used to:

- Clean and transform the raw Netflix dataset
- Handle missing values
- Standardize country and genre information
- Create separate lookup and bridge tables
- Prepare the data for Power Pivot modeling

## 🧩 Data Modeling

Power Pivot was used to create relationships between:

- Netflix main data
- Country lookup table
- Country bridge table
- Genre lookup table
- Genre bridge table

Bridge tables were used because a single Netflix title can belong to multiple countries or genres.

## 📐 DAX Measures

The dashboard uses DAX measures such as:

- Total Titles
- Total Movies
- Total TV Shows

Example:

```DAX
Total Titles =
DISTINCTCOUNT([show_id])
```

```DAX
Total Movies =
CALCULATE(
    DISTINCTCOUNT([show_id]),
    [type] = "Movie"
)
```

```DAX
Total TV Shows =
CALCULATE(
    DISTINCTCOUNT([show_id]),
    [type] = "TV Show"
)
```

## 📈 Dashboard Features

### Movies vs TV Shows
Displays the distribution of Movies and TV Shows using a donut chart.

### Netflix Content Addition Trend
Shows how Netflix content additions changed over the years.

### Top Countries by Netflix Content
Displays countries with the highest number of Netflix titles.

### Top Genres
Shows the most common Netflix content genres.

### Content Rating Distribution
Analyzes Netflix titles based on their content ratings.

## 🎛️ Interactive Filters

The dashboard includes slicers for:

- Type
- Year
- Country
- Genres
- Rating

Users can interact with these filters to analyze different segments of Netflix content.

## 📌 Key Learning

This project helped demonstrate how Excel can be used for end-to-end data analytics, from data preparation and relational modeling to DAX calculations and interactive dashboard development.

## 📁 Files

| File | Description |
|---|---|
| `Netflix_Content_Analysis_Dashboard.xlsx` | Complete interactive Excel dashboard |
| `dashboard-preview.png` | Dashboard preview |

## 👩‍💻 Author

Nandini Sonar
