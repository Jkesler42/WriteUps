<h1>Bandit22</h1>

<b>Goal:</b>

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

<b>Solution:</b>

This challenge is similar to the last challenge. The script that the cronjob gets the md5 hash of a particular string and uses that as the file name that it passes the password to. This makes it easy to run the same command and get the file name to <code>cat</code> for the password.

<details>
	<summary>Flag:</summary>

	jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n

</details>