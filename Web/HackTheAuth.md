# Hack the Auth

> Alex's friend sent him a website that stores the data of many Billionaires. But he doesn't know the username and password to log in. Help him win the bounty prize by getting the credentials. [Website link](https://wec-ctf-2022-web.herokuapp.com/q1)

Inspect element and look at the authentication function. The user is `admin` and the password has a hash value of `dfbec338b51c5643ba481625e1075236d3a9a07fbd6393763f253e99024958a4`. Use a rainbow table tool like [CrackStation](https://crackstation.net/) to find the password. Log in with these credentials and get the flag from checking the cookies.

The flag is `CTF{SHA256_AND_WEB}`
