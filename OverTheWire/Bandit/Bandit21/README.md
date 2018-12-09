<h1>Bandit21</h1>

<b>Goal:</b>

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

<b>Solution:</b>

We find a bandit22 crontab file in the folder described. We don't have permissions to use <code>crontab</code> but we can <code>cat</code> that file. A particular bash script is running that outputs the password for bandit22 to a file in the /tmp/ directory. We can <code>cat</code> that file to get the password.

<details>
	<summary>Flag:</summary>

	Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI

</details>