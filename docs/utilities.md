# Online Utilities 

## Recipes

## Backup/Restore
The Backup/Restore utility allows you to save your settings and/or your processes to a local drive on your computer. 

### Backup
To backup your configuration, click on the Backup/Restore tab at the top of the screen.

![backup_restore](img/backup/backup_restore_tab.png)

Enter the IP address for your BCS. The utility will locate your BCS and display the elements that are available for backup. Choose which settings you want to include in the backup by checking or unchecking the check boxes. The **System Settings** include any custom settings you have configured such as custom names for temperature probes and processes. The **Processes** are the actual processes you have configured on your system.

Enter a name for the backup file. Click the Begin Backup button. The backup file creation will take a minute to complete. Select a location on your local machine where you want to save the file to finish the process.

![backup](img/backup/backup.png)

### Restore
To restore from a previously save configuration, click on the Restore tab. Enter your BCS IP address. Click the **Choose File** button and open the configuration file from which you want to restore. Click on the **Restore Backup** button.

![restore1](img/backup/restore1.png)

Once the utility reads the file, you can choose to restore the Settings and/or individual processes. In addition, you can map the processes in the backup file to different process numbers on your BCS. Once you are satisfied with your choices, click the **Restore Backup** button to complete the process. The restore process will take a few minutes to complete. Once the restore process has completed, you need to reset the BCS for the changes to take effect. Go to the [Settings](settings.md) page and click on the **System Reset** button.

![restore1](img/backup/restore2.png)


## 3.x Config Migrator
The Config Migrator allows you to import your existing BCS 3.x configuration into 4.0. To begin, you must first have a 3.x backup file. 

Navigate to the 3.x Migrator utility. Enter the IP address of your BCS. Click on the **Choose File** button and select your 3.x backup file. Click on the Begin Migration button. Once all the configuration parameters are shown as **Done**, you can close the progress window.  Once the migration process has completed, you need to reset the BCS for the changes to take effect. Go to the [Settings](settings.md) page and click on the **System Reset** button.

## PID Tuner



