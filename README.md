# DataProcessingTool

Data Processing Tool principles of operation:
1. Backup is created automatically after every significant change in the data composition. There is no need to backup state manually 
2. To roll back to any of the previous data states, Restore button should be used 
3. Data is stored in the local MongoDB instance
4. Pre-processed CSV files are stored in JSON files in the notebook folder
5. Aggregated data is exported to HTML files (notebook folder)
6. 
