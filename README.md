# JJ-cookbook

Here I will talk about using the tool FFUF(Fuzz faster u fool).
It is a fast web fuzzer written in go language and it can be downloaded from below given github:
https://github.com/ffuf/ffuf

We can perform directory discovery with ffuf along with tasks like virtual host discovery.
We can use the following syntax for directory discovery:

ffuf -c -w /path/to/wordlist -u https://target/FUZZ

We can fuzz host headers by using the following:

ffuf -w hosts.txt -u https://example.org/ -H "Host: FUZZ" -mc 200
