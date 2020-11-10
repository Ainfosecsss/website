

SiMon 

11/10/2020

- dataengine  

[BUGFIX] Fix potential "mmap: invalid argument" errors in loading the head chunks, after an unclean shutdown, by performing read repairs. #8061
[BUGFIX] Fix serving metrics and API when reloading scrape config. #8104
[BUGFIX] Fix head chunk size calculation for size based retention. #8139
 
- pushgateway 

[UPDATE] jQuery again. Currently used 3.4.1, which has known XSS vulnerabilities:
	* https://nvd.nist.gov/vuln/detail/CVE-2020-11022
	* https://nvd.nist.gov/vuln/detail/CVE-2020-11023
		


