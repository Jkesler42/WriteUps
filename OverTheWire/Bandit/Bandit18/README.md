<h1>Bandit18</h1>

<b>Goal:</b>

The password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

<b>Solution:</b>

To get around getting logged off we can pass the <code>cat</code> command directly into the ssh command like so: 

<code>ssh servername -p port -l bandit18 "cat readme"</code>

This will read that file and pass it back before .bashrc logs the session out.

<details>
	<summary>Flag:</summary>

	IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

</details>