<h1>Bandit29</h1>

<b>Goal:</b>

There is a git repository at ssh://bandit29-git@localhost/home/bandit29-git/repo. The password for the user bandit29-git is the same as for the user bandit29.

Clone the repository and find the password for the next level.

<b>Solution:</b>

Again the password is missing from the file in the repo. There aren't any other useful commits in the master branch. Using <code>git branch -a</code> we can see there is a dev branch. Checking that branch out lets us get the password from the file.

<details>
	<summary>Flag:</summary>

	5b90576bedb2cc04c86a9e924ce42faf

</details>