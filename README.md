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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/97210eb4-5021-41f9-97aa-a2bdb1b852b7)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/9060900b-c3b7-4e58-a1a7-829bc3e5ad18)
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/4d28761a-0ffd-437b-99fb-d07498293fae)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/ef408710-a642-40e3-ab9e-ccb65c057c4f)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/a3cbe2ca-425c-46e9-9621-cb4f6d231ff3)
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/797ab606-c163-414a-8a5d-b164c624247f)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/e4042baf-23c3-454b-8e10-744573666a14)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```


## OUTPUT
![image](https://github.com/SusithraB/Windows-basic-commands-batchscript/assets/146347839/73877fa2-c82c-41f1-8e40-6ada9531e141)

# RESULT:
The commands/batch files are executed successfully.

