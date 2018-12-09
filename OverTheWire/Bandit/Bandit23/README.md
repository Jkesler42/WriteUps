<h1>Bandit23</h1>

<b>Goal:</b>

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

<b>Solution:</b>

This challenge is similar to the prior two challenges. We have to put a script in a directory. A cronjob will run any scripts in that directoy once a minute. I used this script below to <code>cat</code> the password file. The only issue I had was messing around with permissions on the destination folder but finally figured out my issue.

<code>#!/bin/bash

cat /etc/bandit_pass/bandit24 >> /tmp/<i>mydir</i>/pass.txt
</code>

<details>
	<summary>Flag:</summary>

	UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ

</details>