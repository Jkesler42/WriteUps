<h1>Bandit9</h1>

<b>Goal:</b>

The password for the next level is stored in the file data.txt in one of the few human-readable strings, beginning with several ‘=’ characters.

<b>Solution:</b>

The data file in this challenge is actually a binary file. We can use <code>strings</code> to extract human readable strings from the file and then <code>grep</code> for multiple "=".

<code>strings data.txt \| grep ==</code>

<details>
	<summary>Flag:</summary>

	truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

</details>