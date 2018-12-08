<h1>Bandit1</h1>

<b>Goal:</b>

The password for the next level is stored in a file called - located in the home directory

<b>Solution:</b>

- is used as a synonym for stdin. Whenever you try to call <code>cat</code> on a file with - as a name it thinks you're talking about stdin. To get around this I simply called <code>cat ./-</code> to give cat context that I was looking for a file named - and not stdin.

<details>
	<summary>Flag:</summary>

	CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
</details>