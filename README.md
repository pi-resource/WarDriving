# WarDriving

Please check out http://www.pi-resource.com/?page_id=378 for full details of this project.

Script to automate the uploading of Kismet WarDriving logs.

The Following actions are performed:
  1. Check directory structure exists, if it doesn't, create it
  2. Stop kismet server to force it to write out the log files
  3. Move kismet log files to an alternative directory
  4. Start Kismet Server
  5. Check is any files require compression, if so, compress them
  6. Check if we have files to upload and an internet connection. If so, upload them
  8. Check disk space, delete old logs if running low
  9. Wait a set amount of time before restarting this script

The script can be configured to upload the data to:
  1. https://www.wigle.net/
  2. http://www.pi-resource.com/
  3. An FTP server specified by you

Changes since last version:

User configuration separated out from main bash script. Configuration file - WarDriving.cfg
An example config file is provided in WarDriving.cfg.example
