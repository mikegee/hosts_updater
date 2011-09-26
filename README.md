HOSTS File Updater
==================

This script downloads the latest HOSTS file from mvps.org, cleans it up a bit,
and appends it to your hosts file.

Run Periodically
----------------

I recommend running this monthly via a cron job.

Here's the line in my crontab:

    0 2 9 * * cd /home/gee/projects/hosts_updater; ./update >>update.log 2>&1

That runs the script at 2am on the 9th of every month.
