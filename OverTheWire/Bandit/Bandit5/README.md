<h1>Bandit5</h1>

<b>Goal:</b>

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

    human-readable
    1033 bytes in size
    not executable


<b>Solution:</b>

This challenge is to find a file using some of it's attributes. Luckily the <code>find</code> command can filter by each of these.

The final command:

<code> find . -size 1033c -type f ! -executable -exec file {} +</code>

The size switch the the "c" on the end denotes the size of the file in bytes. The type switch f means we're searching for regular files. Luckily this finds only one match. If we found multiple matches we could pipe this to <code>grep ASCII</code> to only see human readable files.

<details>
	<summary>Flag:</summary>

	DXjZPULLxYr17uwoI01bNLQbtFemEgo7

</details>