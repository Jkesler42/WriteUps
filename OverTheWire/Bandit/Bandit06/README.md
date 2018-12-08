<h1>Bandit6</h1>

<b>Goal:</b>

The password for the next level is stored somewhere on the server and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size


<b>Solution:</b>

This challenges is similar to the bandit5 challenge. 

<code>find / -size 33c -readable -user bandit7 -group bandit6 -exec file {} +</code>

The biggest difference between this solution and the previous is that you are running find on the root directory (/) instead of the current directory (.).

<details>
	<summary>Flag:</summary>

	HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

</details>