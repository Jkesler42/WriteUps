<h1>Bandit4</h1>

<b>Goal:</b>

The password for the next level is stored in the only human-readable file in the inhere directory. 

<b>Solution:</b>

There are only 10 files to check so bruteforcing this challenge is possible but that is boring so I decided to script a solution.

<code>for i in \*; do file ./$i; done</code>

This oneliner iterates over every file in the directory (all 10 of them) and runs the <code>file</code> command on them.

All but one of the files returns as type data while one returns as type ASCII text.

<details>
	<summary>Flag:</summary>

	koReBOKuIDDepwhWk7jZC0RTdopnAYKh

</details>