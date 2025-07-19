# 🎬 TMDb Movie Dataset Analysis & Visualization

This project was completed as part of the **STAT288: Data Visualization** course at the University of Bahrain.  
It explores patterns in movie preferences, ratings, and genre characteristics using comprehensive visualization techniques.

## 👥 Team
- **Ebrahim Juma Shakak Alsawan**
- **Sadeq Jaafar Ali Deyab**
- **Salman Wael Salman Ahmed** 


## 🎯 Objective
To detect patterns related to people's movie preferences, revenue trends, and how various factors (genres, budget, production variables) affect movie outcomes through effective data visualization.

## 📊 Dataset Overview
**Source**: TMDb 5000 Movie Dataset from Kaggle  
**Size**: 4,803 movies with comprehensive metadata including:
- Movie details (budget, revenue, runtime, ratings)
- Cast and crew information (106,257 cast entries, 129,581 crew entries)
- Genre associations (12,160 genre mappings)
- Production details (countries, companies)

## 🔍 Key Findings

### Genre Quality Patterns
- **Best performing genres**: War (45%), History (42%), Western (40%)
- **Worst performing genre**: Horror (8% good movies)
- **Definition**: "Good movies" = average rating ≥ 7.0 with ≥30 votes

### The Niche Genre Theory
Discovered a **logarithmic relationship** between movie count and quality:
```
Good Movies % = 71.93 - 7.84 × ln(Movie Count)
```
- Niche genres (fewer movies) → Higher quality ratings
- Popular genres (more movies) → Lower average ratings

### Notable Exceptions
- **Drama**: Outperforms expectations despite high movie count
- **Horror**: Underperforms significantly compared to moderate movie count

## 🛠 Tools & Techniques Used
- **Python**: Data cleaning, statistical analysis, correlation matrices
- **Tableau**: Interactive scatter plots and relationship visualizations
- **Pandas**: Data manipulation and cross-tabulation
- **Matplotlib/Seaborn**: Heat maps and bar charts

## 📈 Visualizations Created
1. **Horizontal Bar Chart**: Percentage of good movies by genre
2. **Correlation Heat Map**: Genre associations and co-occurrence patterns  
3. **Scatter Plot**: Movie count vs. quality percentage with logarithmic trendline

## 🔗 Genre Correlation Insights
- Good genres tend to correlate positively with other good genres (History ↔ War)
- Bad genres cluster together (Horror ↔ Thriller ↔ Action)
- Drama acts as a "bridge genre" - correlates with quality genres while maintaining high volume

## 📁 Project Structure
```
├── movies.csv                    # Main movie dataset (4,803 movies)
├── movie_genre.csv              # Genre associations (12,160 mappings)
├── movie_cast.csv               # Cast information (106,257 entries)
├── movie_crew.csv               # Crew details (129,581 entries)
├── movie_country.csv            # Production countries (6,436 entries)
├── movie_company.csv            # Production companies (13,677 entries)
├── data_cleaning.py             # Data preprocessing and transformation
├── python_visualizations.py     # Statistical analysis and plotting
└── report.pdf                   # Complete analysis report
```

## 🎬 Storytelling Narrative
**"Why Does Movie Quality Vary So Dramatically Between Genres?"**

Our analysis reveals that genre quality differences stem from audience targeting strategies rather than inherent genre characteristics. Niche genres succeed through focused storytelling for specific audiences, while mass-market genres sacrifice quality for broader appeal.

---
