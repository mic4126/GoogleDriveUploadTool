# Google Drive Upload Tool
A tool for Windows to upload files to Google Drive. It resumes uploads in case of an error or failure. Perfect for uploading large files or if your connection is unstable. Additionally, files uploaded with this tool will preserve their Modified Date. Also, the software lists the latest uploads and allows you to download them to a chosen folder.

# How to use?
1. Before using this software, follow the Step 1 (Step 1: Turn on the Drive API) in this quick start guide from Google: https://developers.google.com/drive/v3/web/quickstart/dotnet
2. After following the steps, launch the software. It will launch a web tab in your browser to allow the software to access your account.
3. Start uploading or downloading a file!

# How to upload a file or folder?
1. drag and drop one or more file or folder
2. press "Upload". 

* When uploading folders that contains subfolders and subfiles, The original file and folder structure will be kept in Google Drive.
* If an upload is interrupted or the software or the PC crashes, you'll be prompted to continue the upload where it left of if you are uploading the same file as before. If you attempt to upload another file after the first one got interrumpted, you will lose the ability to resume the previous file. If the software is still open and the connection is interrupted, it will attempt to continue the upload.

# How to select a folder?
1. Press "Browse Folder.
2. Select a folder OR if you want to select a subfolder, double click a folder.
3. Press "Select" when you chose the folder you'd like to upload files to.

# How to create a folder?
1. Press "Browse Folder"
2. Press "New"
3. Type a Folder Name and press OK

# How to check if Folder ID is correct?
1. Type Folder ID in the Text Box
2. Press the "Get Folder Name" button
3. If the Folder ID is correct, you'll see the Folder Name in the Text Box below the Folder ID. If the Folder ID is incorrect or not found, a message will be shown telling that the Folder ID is incorrect.

# How to download a file?
1. Choose a file from the list
2. Press the "Download File" button.
3. Choose a folder and if you want, change the filename and press "Save"
4. The download will start

# How to save a Checksum file?
1. Select a file
2. Press the "Save Checksum File" button

To save the checksums for more than 1 file:
1. Select more than 1 file holding either Ctrl or Shift with the keyboard and selecting the files with the mouse
2. A new button will appear right next to "Refresh List"
3. Press the new button called "Save Checksums for selected files".

These are the checksums for your files stored in Google Drive. You can use them to verify if the uploaded file matches the local file.

# How to open and compile the project?
This project was made using Visual Studio 2017, in the Visual Basic .NET language. You'll need to have the Windows Desktop components installed to be able to open and edit this project to fit your needs and to compile it. It also uses the Google Drive API which is available in the NuGet Package Manager. You may also be prompted to download the NuGet packages for this project.

Enjoy!!!

# Changelog:
v1.6 (5/7/2017)
- Software now remembers the folders created when there are still uploads pending
- Software now displays the Folder Name from the entered Folder ID when the software is launched
- Browse files and folders with the same structure as your Google Drive
- See file details
- Folder Browsing has been integrated in the Main Window. Select a folder to upload files to it.
- Save Checksum file to test local file against uploaded file

v1.5 (3/23/2017)
- Changed "Length" to "File Size"
- Added comma in file size (ex. 10,000.00 MB instead of 10000.00 MB)
- When an error occurs, the upload will be retried automatically and also resume from the point it was interrupted.
- Searches for every file and folder inside a folder to upload. The uploads maintain the same structure
- Option to preserve file modified date added.
- Can now browse and create Folders to upload files
- If copy/pasting folder ID from Google Drive, you can now press the Get Folder Name button to get the folder name based on its ID
- Can drag and drop more files to upload to queue while uploading
- Can select more than one file or folder to remove
- Can now erase the entire upload list
- Timeout reduced to 2 minutes (120 seconds). Should be enough as the chunk size was reduced to 1MB in v1.2

v1.4 (3/20/2017)
- Added Batch Upload
- Uploaded Items list now shows 25 items per page

v1.3.1 (3/19/2017)
- Files get uploaded with the original file Modified Date

v1.3 (3/19/2017)
- Added Spanish Language

v1.2 (3/19/2017)
- Upload files to a Folder ID
- Added Time Left for Upload/Download
- Chunk Size reduced to 1MB to prevent timeout issues with slower internet connections

v1.1 (3/19/2017)
- Lists files in ListBox
- Can download a selected file to a chosen directory
- Can drag and drop a file to upload

v1.0 (3/18/2017)
- Initial Release
- Ability to upload a file and resume if interrumpted
