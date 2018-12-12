<h1>Bandit25</h1>

<b>Goal:</b>

Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

<b>Solution:</b>

They give you the SSH key to login to bandit26. The problem is that logging directly into bandit26 prints some text and then exits out immediately. Checking the /etc/passwd file, we see the default shell isn't /bin/bash. The login script is:

<code>\#\!/bin/sh

export TERM=linux

more \~/text
</code>

So it runs <code>more</code> on some text file which eplains the text that appears when attempting to login. (I needed a hint at this part.) More only stops if the output goes past the bottom of your screen. If you shrink your screen to be only a couple lines, the script will stop until you press a button. This is important. If you hit v while more is running, a vi editor will open with that file. Then you can use vi to run a shell with :shell. This is a classic way to escape certain restricted shells. 

With this shell we can <code>cat</code> the password text file to get the actual password to bandit26. We also need this shell for bandit27.

<details>
	<summary>Flag:</summary>

	5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z

</details>