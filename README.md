Google-Drive-Download
Python scripts to download folders and files from google drive

Pre-requisites - Authorize API usage on google drive, and download/install google drive pyhton api. 
sudo pip install -I google-api-python-client==1.3.2 --ignore-installed six
Authorize API https://developers.google.com/drive/v3/web/quickstart/python#step_1_turn_on_the_api_name
Download the client_secret.json to same dir as this script
Made for Python 3.5 and Google Drive API v3.

Usage: to replicate a Gogle Drive folder structure with all files, in your computer
python dl_gdrive_folder.py <Google drive folder source> <local computer folder destination>
Example:
Folder Structure at Google Drive:
F1
	File0
	F11
		File1
	F12
		F211
			FileA
			FileB
To download everything from folder F211 to a local folder TST
python dl_gdrive_folder.py F211 TST	


Build from the works of :
Mark Culhane - google_drive_backup.py
https://github.com/markz0r/tools/blob/master/backup_scripts/google_drive_backup.py
and
HatsuneMiku - recursive navigation over folders
http://stackoverflow.com/questions/22092402/python-google-drive-api-list-the-entire-drive-file-tree
https://github.com/HatsuneMiku/googleDriveAccess





