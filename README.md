# 📄 Summary

The raw marketing campaign dataset was initially loaded into the environment, but it appeared in a messy form where all values were merged into a single column. To convert this into a usable format, the data was split into multiple columns using the tab delimiter. The first row of this split data contained the actual column names, so it was extracted and assigned as the header of the dataset, after which the index was reset to ensure a clean and structured dataframe.

Once the dataset structure was organized, an inspection was carried out to understand the data types, column counts, and overall shape of the dataset. The dataset was also checked for duplicate records to ensure the integrity of the data, followed by a check for missing values to identify any gaps that needed to be handled before further analysis.

Since many columns were in string format but represented numerical values, type conversion was performed. All non-categorical columns were converted into numeric format, and any invalid or empty values were safely converted to zeros. After this conversion, the numerical columns were cast into integer type to maintain consistency throughout the dataset. The date column, Dt_Customer, which contained customer enrollment dates, was also converted into a proper datetime format to enable time-based analysis.

By the end of this cleaning process, the dataset was fully structured, free of duplicates, consistent in data types, and ready for exploratory analysis or model building. The final dataset contains 2240 records across 29 well-formatted columns
