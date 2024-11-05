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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![330012900-c65ec521-e638-4a1f-8bdd-97c56e1efc85](https://github.com/user-attachments/assets/66e49689-9155-4780-966b-a9a3e042f4be)




## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![330013412-b9be78f6-9828-4e71-a5a9-f6f1189783ed](https://github.com/user-attachments/assets/ffaff5a3-bf23-4b9d-94ce-96a0f8c81686)
```
type nul > MyFile.txt
```
![330013653-bd325e68-6b4b-4534-8545-4a27ff88884b](https://github.com/user-attachments/assets/4decb688-4355-45dd-b13d-cd83b2b8631c)




## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![330012712-30682b3a-8a3a-42f2-a0ce-4e01779085c9](https://github.com/user-attachments/assets/d5106ef9-6420-4bbd-bbbd-cb4d60a0660d)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
```
![330012322-64b3d1fb-6b15-47d7-b449-18d1df73456e](https://github.com/user-attachments/assets/a3a4cb6e-c598-4125-950a-e208de9ab3e8)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![330012410-6a48ce78-88e9-4a7e-a2e5-8ece42f7311e](https://github.com/user-attachments/assets/2d015b6f-bbe6-47b0-b732-db64c2c342d2)



## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```
![330012125-1b3b3dfc-19ad-4574-98e2-e28bd46533f1](https://github.com/user-attachments/assets/be205bed-877f-4c31-840a-3096ffbb2e60)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## comand
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![330011170-759f68b0-4717-4bea-9e37-4f8bc436e3b6](https://github.com/user-attachments/assets/efb2981b-8f29-423d-bf97-b5baeb71ebe9)


## command
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```









## OUTPUT

![328877014-777c22b5-a3b1-444f-ad7a-045c05cd0d9c](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/d7e77e7f-05ef-4e45-bb32-2e4df33c98f2)




# RESULT:
The commands/batch files are executed successfully.

