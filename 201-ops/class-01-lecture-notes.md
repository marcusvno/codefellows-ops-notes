# 201 Intro to Computer Fundamentals - Class 01 Lecture Notes

## Backing Up Your System

***Systems are replacable. Data is sacred!***

### Backup Strategy

An effective Backup Strategy considers:
- Data Inventory and Classification
- Backup Types 
- Location, Redundancy, and Replication
- Frequency and Scheduling
- Monitoring and Testing
   - Backups are **UNPROVEN** until they have been *fully tested.*
- Disaster Recovery Plan

### Backup Types

- Normal / Full
   - Replicates Everything. Comprehensive backup.
   - Good for your first time doing a backup
   - High Backup time / Low restore time

- Incremental 
   - Saves only the changes from the last INCREMENTAL backup.
   - Low backup time/ high restore time

- Differential 
   - Saves what's changes since the last FULL back up.
   - Moderate backup time / moderate restore time.

### Offsite Backups

**Offsite Backups** are data backups stored in a different geographic location than the production system.

- **Hot Site**
   - Most expensive option.
   - An exact duplicate of the production site, ready to take over immediately if production site fails.

- **Cold Site**
   - Takes a long time to spin up.
   - Less costly than *hot sites.*

