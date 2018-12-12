<h1>Bandit28</h1>

<b>Goal:</b>

There is a git repository at ssh://bandit28-git@localhost/home/bandit28-git/repo. The password for the user bandit28-git is the same as for the user bandit28.

Clone the repository and find the password for the next level.


<b>Solution:</b>

This challenge seems straight forward but there are a couple extra steps. When you clone the repo and cat the file the password has been sanitized. Run <code>git log</code> to check prior commits. Sure enough there is a commit with a comment about a data leak. We <code>git reset --hard commithash</code> to get the unsanitized file.

<details>
	<summary>Flag:</summary>

	bbc96594b4e001778eee9975372716b2

</details>