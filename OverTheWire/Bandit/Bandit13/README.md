<h1>Bandit13</h1>

<b>Goal:</b>

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

<b>Solution:</b>

Bandit14's private key is in the home directory of Bandit13. Copy the file back to your computer and use <code>ssh -i</code> to use the key file to login to bandit14. Once logged in to bandit14 we can go back and get the actual password from /etc/bandit_pass/bandit14.

<details>
	<summary>Flag:</summary>

	4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

</details>