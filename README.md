# Stack Overflow Developer Survey EDA
**Category:** Data Science  
**Tech Stack:** Python, Streamlit, Plotly, Pandas, NumPy  
**Status:** Complete  
**Thumbnail:** assets/thumbnail.png
## Overview
An interactive Streamlit dashboard for exploring the Stack Overflow Developer Survey 2023 data. Visualize developer demographics, technology preferences, AI tool adoption, and salary insights through multi-page interactive charts with smart data processing for complex survey responses.
## Features
- **Multi-Page Dashboard**: 8 analysis pages including demographics, tech tools, AI adoption, and Stack Overflow usage
- **Smart Data Processing**: Custom parser handles semicolon-separated multi-choice survey responses
- **Interactive Visualizations**: Bar charts, pie charts, and line graphs with Plotly
- **Auto Label Encoding**: Smart compression for categories with 30+ unique values to prevent chart clutter
- **Data Quality Filtering**: Automatically removes incomplete responses (rows with >40 missing values)
- **Performance Caching**: Streamlit data caching for fast dashboard loading
## Project Structure
```
skilharvest_stackoverflow_eda/
├── survey.py                     # Main Streamlit application
├── plot.py                       # Plotting utilities and data processors
├── survey_EDA.ipynb              # Jupyter notebook exploration
└── README.md
```
## Dataset
**Stack Overflow Developer Survey 2023**
- 89,000+ developer responses
- 84 columns covering demographics, education, work experience, technology stack, AI tools, compensation
- Multi-choice questions with semicolon-separated values
## Analysis Pages
| Page | Insights |
|------|----------|
| **Basic Information** | Age, employment, education, experience |
| **Tech Tools** | Programming languages, databases, frameworks |
| **AI Tools** | AI adoption, sentiment, tools used |
| **Stack Overflow** | Usage frequency, community participation |
| **More AI** | Detailed AI analysis |
| **Group By** | Comparative analysis |
## Getting Started
### Prerequisites
- Python 3.8+
- Streamlit
### Installation
```bash
git clone https://github.com/aniekanudo-MD/skilharvest_stackoverflow_EDA.git
cd skilharvest_stackoverflow_eda
pip install streamlit pandas numpy matplotlib seaborn plotly
```
### Run the Dashboard
```bash
streamlit run survey.py
```
The app opens at `http://localhost:8501`
## How It Works
1. **Data Loading**: Reads Stack Overflow survey CSV with caching
2. **Data Cleaning**: Filters incomplete responses, fills missing values
3. **Response Parsing**: Extracts individual choices from semicolon-separated strings
4. **Visualization**: Generates bar/pie/line charts based on column type
## Tech Stack
- **Framework**: Streamlit
- **Visualization**: Plotly Express
- **Data Processing**: Pandas, NumPy
- **Charts**: Matplotlib, Seaborn
## Contact
- **Email**: [Aniekan Udo @Gmail](mailto:aniekanetimudo+reachout@gmail.com)
- **LinkedIn**: [Aniekan Udo @Linkedin](https://www.linkedin.com/in/aniekan-etim-udo)
## License
MIT
