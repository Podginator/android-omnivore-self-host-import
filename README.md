# Omnivore Data Exporter from Android

Omnivores android app stores the contents of the application in an omnivore-database file. This includes all the saved links, whether they are archived and their tags. 

This python notebook aims to take those files, and export them to a self-hosted instance. 

This was tested using the android emulator. I believe you may need root to access the files needed for this.
https://www.airdroid.com/file-transfer/access-android-data-folder-without-root/ This article implies it is possible without. 

Omnivore parses articles asynchronously, and when they're finished parsing they update the archive status and savedAt status. It may therefore be necessary to run the final step of this project more than once. 

To run this create a python venv, install the requirements.txt and run `jupyter notebook`. 