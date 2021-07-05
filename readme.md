
# Nat Monitor
##### Procedure for configuring Linux scheduler:
##### root@sayeed:/##### crontab -l   view scheduled tasks
##### root@sayeed:/##### crontab -e   edit scheduler
##### Add the following line to run the script every 5 minutes, every hour, every day, every month:
##### */5 * * * * /path_to_file/NetMon_SQL_v1.py /path_to_file/NETWORK_IP /path_to_file/SSH_USERPASS.txt /path_to_file/SQL_CONN.txt
##### For more info about configuring scheduler: http://kvz.io/blog/2007/07/29/schedule-tasks-on-linux-using-crontab/
##### Before scheduling this task, run the script in the console to check for errors:
##### Go to the folder containing the script and all files, using cd /netmon_folder_path
##### Enter this command: python NetMon_SQL_v1.py NETWORK_IP.txt SSH_USERPASS.txt SQL_CONN.txt
##### Check the console output and SQL_Error_Log.txt file for any errors.
##### Running the script is recommended at intervals of at least 5 minutes.

# Logical Flow Diagram
![](https://i.ibb.co/1RJS9Vw/flowdiagram.jpg)