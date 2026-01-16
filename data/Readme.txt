Netflix Data Cleaning Project - Excel Basics
Task 1: Data Analyst Internship

Project Overview
This project involves cleaning and formatting a raw dataset of Netflix Movies and TV Shows (approx. 8,000+ rows). The goal was to transform "messy" data into a structured, analysis-ready format using Microsoft Excel.

Dataset Details
Source: Kaggle (Netflix Movies and TV Shows)

Format: CSV / XLSX

Initial State: Contained missing values, inconsistent date formats, and placeholder text ("Not Given").

Step-by-Step Cleaning Process
Phase 1: Setup and Inspection
Data Segregation: Created two tabs: Raw_Data (original) and Cleaned_Data (working sheet) to ensure data integrity.

View Optimization: Applied Freeze Panes to the header row and enabled Filters across all columns for easy navigation.

Phase 2: Handling Missing Values & Placeholders
Identifying Gaps: Used Conditional Formatting to highlight blank cells in red.

Standardizing "Not Given": Found that many cells contained the text "Not Given" instead of being truly blank. Used Find & Replace (Ctrl+H) to change these to "Unknown" for better categorization.

Imputation: For the Director and Cast columns, missing values were filled with "Not Specified" to avoid losing valuable row data.

Phase 3: Data Standardization
Date Formatting: The date_added column had multiple formats (e.g., MM/DD/YYYY, DD-Mon-YY, and text).

Used the Text-to-Columns wizard (Date: MDY) to force Excel to recognize all entries as dates.

Applied a uniform date format (YYYY-MM-DD) to the entire column.

Text Cleaning: - Applied the TRIM function to the title and description columns to remove accidental leading or trailing spaces.

Used PROPER on category columns to ensure consistent capitalization (e.g., "movie" became "Movie").

Phase 4: Deduplication & Validation
Removing Duplicates: Used the Remove Duplicates tool based on the show_id and title columns to ensure every entry is unique.

Data Type Validation: Verified that release_year was formatted as a Number and type was a consistent Category.