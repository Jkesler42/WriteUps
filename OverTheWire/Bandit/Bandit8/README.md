<h1>Bandit8</h1>

<b>Goal:</b>

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

<b>Solution:</b>

Using <code>uniq</code> we are able to see lines that only occur once. <code>uniq</code> only works on adjacent lines so first we have to use <code>sort</code> to group the lines correctly.

<code>sort data.txt \| uniq -u</code>

<details>
	<summary>Flag:</summary>

	UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

</details>