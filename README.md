# Spotify Trending Music Data Analysis Project

## 📊 Project Overview

This project analyzes Spotify trending music data collected from multiple playlists and markets worldwide. We collected over 3,600 tracks from 50+ playlists across 11+ countries, performed comprehensive data cleaning and preprocessing, conducted exploratory data analysis, statistical hypothesis testing, and applied machine learning techniques including K-means clustering and PCA to uncover patterns in global music trends.

## 🎯 Key Features

- **Data Collection**: Automated collection from 50+ Spotify playlists across multiple markets
- **Data Cleaning**: Comprehensive preprocessing and duplicate removal
- **Exploratory Data Analysis**: Distribution analysis, correlation matrices, and visualizations
- **Statistical Analysis**: Hypothesis testing, feature engineering, clustering, and PCA
- **Comprehensive Reporting**: Professional markdown report with insights and visualizations

## 📈 Dataset Statistics

- **Total Tracks Collected**: 3,601 tracks
- **Unique Tracks**: 2,863 tracks (after duplicate removal)
- **Markets Covered**: 11+ countries (US, Japan, India, Brazil, UK, Germany, etc.)
- **Playlists Analyzed**: 50+ playlists including Top 50 and Viral 50 charts

## 🚀 Quick Start

### Prerequisites

```bash
pip install -r requirements.txt
```

### Data Collection

```bash
python collect_spotify_trending.py
```

This will collect data from multiple Spotify playlists. The script will:
- Search for playlists by name
- Collect track metadata and audio features
- Save data to timestamped CSV files

### Data Analysis

```bash
python data_analysis.py
```

This will run the complete analysis pipeline:
1. Data loading and cleaning
2. Exploratory Data Analysis (EDA)
3. Statistical analysis
4. Insight generation

The analysis automatically generates visualizations and saves them to the `analysis_output/` directory. The comprehensive markdown report (`DATA_ANALYSIS_REPORT.md`) is included in this repository.

## 📁 Project Structure

```
.
├── collect_spotify_trending.py    # Data collection from Spotify API
├── data_analysis.py               # Main analysis pipeline
├── requirements.txt                # Python dependencies
├── README.md                      # Project documentation
├── DATA_ANALYSIS_REPORT.md        # Comprehensive analysis report
├── DBA_project_2022517.pdf        # Final project report (PDF)
├── analysis_output/                # Analysis results
│   ├── processed_data.csv         # Cleaned dataset
│   ├── basic_statistics.csv       # Summary statistics
│   ├── insights.txt               # Key insights
│   └── *.png                      # Visualization files (11 figures)
└── [Raw CSV files excluded - can be regenerated]
```

## 📊 Analysis Outputs

All analysis outputs are saved in the `analysis_output/` directory:

### Visualizations
- `feature_distributions.png` - Distribution of key audio features
- `correlation_matrix.png` - Correlation heatmap of audio features
- `top_artists.png` - Top 20 artists by track count
- `collaboration_distribution.png` - Collaboration vs solo tracks
- `market_distribution.png` - Track distribution by market
- `playlist_distribution.png` - Track distribution by playlist
- `release_year_trend.png` - Release year trends
- `release_month_distribution.png` - Release month patterns
- `popularity_vs_features.png` - Popularity vs audio features scatter plots
- `mood_distribution.png` - Mood classification
- `audio_features_boxplot.png` - Box plots of audio features

### Data Files
- `processed_data.csv` - Cleaned and processed dataset with engineered features (2,863 unique tracks)
- `basic_statistics.csv` - Descriptive statistics for all numeric features
- `insights.txt` - Summary of key insights from the analysis

## 🔑 Key Findings

### Top Artists
- **Most Featured Artist**: Nusrat Fateh Ali Khan (51 tracks)
- Other top artists include Umur Anil Gokdag, Karan Aujla, The Weeknd, Ariana Grande, and Taylor Swift

### Market Distribution
- **Top Markets**: US (247 tracks), Japan (134), India (127), Brazil (107), UK (96)
- Data collected from 11+ countries worldwide

### Collaboration Analysis
- **Collaboration Rate**: 38.8% of tracks are collaborations
- Mean popularity: Collaborations (49.54) vs Solo (47.77)

### Temporal Trends
- **Peak Release Year**: 2025 (705 tracks), 2024 (500 tracks), 2023 (510 tracks)
- Most releases in February (306 tracks) and January (294 tracks)

## 🛠️ Technical Details

### Technologies Used
- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib & Seaborn** - Data visualization
- **Scikit-learn** - Machine learning (clustering, PCA)
- **Spotipy** - Spotify Web API access
- **SciPy** - Statistical analysis

### API Configuration

The project uses Spotify Web API. Configure your credentials:

```python
SPOTIFY_CLIENT_ID = "your_client_id"
SPOTIFY_CLIENT_SECRET = "your_client_secret"
```

Or set environment variables:
```bash
export SPOTIFY_CLIENT_ID="your_client_id"
export SPOTIFY_CLIENT_SECRET="your_client_secret"
```

## 📝 Analysis Pipeline

1. **Data Collection**
   - Search for playlists by name
   - Collect track metadata (name, artist, album, popularity, etc.)
   - Fetch audio features (danceability, energy, valence, etc.)
   - Handle pagination for large playlists

2. **Data Cleaning**
   - Remove duplicates based on track_id
   - Convert data types
   - Handle missing values
   - Create derived features (duration in minutes, release year, etc.)

3. **Exploratory Data Analysis**
   - Descriptive statistics
   - Distribution analysis
   - Correlation analysis
   - Market and playlist analysis
   - Temporal analysis

4. **Statistical Analysis**
   - Hypothesis testing (collaborations vs solo tracks)
   - Feature engineering (mood classification, popularity categories)
   - K-means clustering
   - Principal Component Analysis (PCA)

5. **Insight Generation**
   - Pattern identification
   - Trend analysis
   - Business insights

## 📄 Reports

The project includes comprehensive documentation:

### Markdown Report (`DATA_ANALYSIS_REPORT.md`)
Complete analysis report with:
- Executive Summary
- Methodology and data collection process
- Data cleaning and preprocessing steps
- Exploratory Data Analysis results
- Statistical analysis findings
- Key insights and visualizations
- Conclusions and recommendations

### Final Project Report (`DBA_project_2022517.pdf`)
The final project report in PDF format, ready for submission.

## 🔗 GitHub Repository

> **Note**: The complete project code, data collection scripts, and analysis pipeline are available in the GitHub repository. Due to dataset size, the raw data files are not included in the repository but can be regenerated using the collection scripts.

**Repository Link**: https://github.com/shadow-112/DS464-semproject-startraders

## 📊 Dataset Information

- **Source**: Spotify Web API
- **Collection Date**: December 2025
- **Total Records**: 3,601 tracks
- **Unique Tracks**: 2,863 tracks
- **Features**: 30+ features including track metadata, audio features, and derived features

## 🤝 Contributing

This is an academic/research project. For questions or contributions, please refer to the GitHub repository.

## 📜 License

This project is for educational and research purposes.

## 👤 Authors

Star Traders  
GIKI  
2022517, 2022605, 2022062

---

**Last Updated**: December 2025

