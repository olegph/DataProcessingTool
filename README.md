# DataProcessingTool

Data Processing Tool principles of operation:
1. Backup is created automatically after every significant change in the data composition. There is no need to backup state manually 
2. Restore of the previous data state is possible on the first step of the processing pipeline (Load button)
3. All data is stored in the local MongoDB instance 
