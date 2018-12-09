<h1>Bandit15</h1>

<b>Goal:</b>

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

<b>Solution:</b>

Since <code>nc</code> doesn't work with ssl, we have to use a different tool to connect to the socket. <code>openssl s_client -connect</code> works for what we need to do.

<details>
	<summary>Flag:</summary>

	cluFn7wTiGryunymYOu4RcffSxQluehd

</details>