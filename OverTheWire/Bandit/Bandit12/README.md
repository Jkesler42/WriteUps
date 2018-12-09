<h1>Bandit12</h1>

<b>Goal:</b>

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. 

<b>Solution:</b>

So we're given a hexdump file. We can turn a hexdump back to a binary file using <code>xxd -r</code> Using <code>file</code> command on the file, we can see the type of compression. Decompress with tar, gzip, or bzip2. Rinse and repeat until we get a human readable ASCII file.

<details>
	<summary>Flag:</summary>

	8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

</details>