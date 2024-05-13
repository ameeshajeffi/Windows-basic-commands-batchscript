# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

name:Ameesha jeffi J

reg no:212223220007

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
## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\MyLab
```
![329658320-0d1c931c-0132-467e-a239-1a645505b196](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/0c8dc067-e4f1-4c9c-b2c3-99c60ef2521c)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
# COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
```

![328876538-072bf08b-8f1f-47e7-9ce0-4bd5389e5e43](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/f7eb7f97-9145-4802-a6d3-7bb059fe62c4)

```
type nul > MyFile.txt
```
![328876592-72daf233-97b8-4bab-829b-4e43929a4fb1](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/58a33048-8cd1-4aae-841e-c6bca9f275a5)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![328876668-ffa2b94b-cc47-478d-aaaf-e07201189f9f](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/c40f1200-2da1-4e72-9f2d-41ceb00df680)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![328876764-b398f90e-ae0b-4acd-9f4c-f61ecfe8cb82](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/d34c5153-5092-4e5b-855f-12cf87c1c4f3)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![328876840-98ab3063-d62a-4eb1-96a3-444a8d8aff5d](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/8fc0ab28-ff1b-43ec-a2e2-056aebe2f50a)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![328877293-342ac881-4ac9-4c2f-a6a0-cdc37248f16c](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/b826c40b-69fc-4008-99bb-2c169caa12ec)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

# COMMAND:

```

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![329660834-0594a6df-84d8-4328-a347-5e6ca215a41c](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/21f72afd-bd92-43ea-8f28-f710964c350a)



# COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

# OUTPUT:

![328877014-777c22b5-a3b1-444f-ad7a-045c05cd0d9c](https://github.com/ameeshajeffi/Windows-basic-commands-batchscript/assets/150773598/4755c9b0-f4b8-44b4-bb35-0bcab2c81426)

# RESULT:
The commands/batch files are executed successfully.

