<h1>Bandit20</h1>

<b>Goal:</b>

There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

<b>Solution:</b>

Echoing the old password to <code>nc -l</code> to create a listening nc connection on a particular port then using that port in the binary provided gets us the new password. Since we only have one window, we have to move the nc command to the bg using ctrl+z and move it back to the foreground with <code>fg</code>

<details>
	<summary>Flag:</summary>

	gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr

</details>