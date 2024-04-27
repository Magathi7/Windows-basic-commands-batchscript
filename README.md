# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it
```
mkdir %userprofile%\Desktop\MyLab

```
![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/b732b111-6397-4c6d-9337-8e006b743b8e)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/b5472d40-1d5f-499b-98be-fbe03be6465c)
![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/1367f007-a1e5-4071-b8a0-112197e59d30)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/ff99a017-2024-4bbf-9e4f-782dcad669a3)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/1646fa08-1ead-4b20-9416-3ce86516c778)
![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/0af75da2-5774-48cf-9077-49cb367b1623)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/4f6abf10-96ae-4c85-b268-d100f7296bea)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```



## OUTPUT

![image](https://github.com/Magathi7/Windows-basic-commands-batchscript/assets/144870480/c4e835aa-34a7-46d5-8690-75dffc666561)




# RESULT:
The commands/batch files are executed successfully.

