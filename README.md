# DataProcessingTool

Setup:
1. Demo dataset (trimmed version of the original one) is supplied and can be used if placed in the notebook folder
2. MongoDB is looking for default config localhost:27017
3. MongoDB dump is included, but will be created on start if not found 

Data Processing Tool principles of operation:
1. Backup is created automatically after every significant change in the data composition. There is no need to backup state manually 
2. To roll back to any of the previous data states, Restore button should be used 
3. Data is stored in the local MongoDB instance and local files
4. Pre-processed CSV files are stored in JSON files in the same folder where source files are
5. Aggregated data is exported to HTML files (notebook folder)
6. Visualisations are generated dynamically every time, data is neither changed or stored 
7. In case dataset is large and number of features is > 50, bottom 20 features in violation dataset are discarded 

What should be done better:
- Move all pre-processing and analysis to the background and on the Transform stage only to make Analyze and Visualize sections responsive
- Add Threads + progress indication in all time-consuming processes
- Make correlation analysis meaningful 
- Either make UI fully interactive with dialog-like mode or switch to options to minimize questions
- Add snapshots management mechanism + status preview for snapshots
