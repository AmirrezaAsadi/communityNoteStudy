# communityNoteStudy

Study community notes using Python data analysis.

## Overview

This repository contains tools for analyzing Community Notes (formerly Twitter Birdwatch) data. Community Notes is a collaborative system that allows users to add context to potentially misleading posts.

## Files

- `community_notes_analysis.ipynb` - Jupyter notebook for loading and analyzing Community Notes data
- `notes-00000-2.tsv` - Sample Community Notes dataset in TSV format

## Usage

### Prerequisites

Install the required Python packages:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Running the Analysis

1. Ensure your `notes-00000-2.tsv` file is in the repository root directory
2. Launch Jupyter Notebook:

```bash
jupyter notebook community_notes_analysis.ipynb
```

3. Run all cells to perform the complete analysis

## Notebook Features

The notebook includes:

- **Data Loading**: Reads TSV files with pandas
- **Data Overview**: Displays dataset structure, columns, and basic statistics
- **Descriptive Statistics**: Comprehensive statistical summary
- **Classification Analysis**: Distribution of note classifications
- **Temporal Analysis**: Time-based trends (if timestamp data available)
- **Visualizations**: Multiple charts including:
  - Classification distributions
  - Missing data patterns
  - Numerical feature distributions
  - Correlation heatmaps
- **Text Analysis**: Word count and content analysis
- **Summary Report**: Key insights and findings

## Data Format

The TSV file should contain Community Notes data with columns such as:
- `noteId`: Unique identifier for the note
- `tweetId`: ID of the associated tweet
- `classification`: Classification of the note (e.g., NOT_MISLEADING, MISINFORMED_OR_POTENTIALLY_MISLEADING)
- `createdAtMillis`: Creation timestamp in milliseconds
- `noteAuthorParticipantId`: Author identifier
- `summary`: Text content of the note
- Additional columns for ratings and metadata

## License

This project is for educational and research purposes.
