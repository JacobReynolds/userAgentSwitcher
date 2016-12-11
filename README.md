#User Agent Switcher

Python script script to check various user agents against the given domain.  It will alert you if any differences are found in how the domain handles user agents.

##TODO
Increase reliability of checks between user-agents, current checks do a full diff.  Website may include timestamps or other things that could cause false positives.

## Installation
```
~$ git clone https://github.com/JacobReynolds/userAgentSwitcher.git
~$ cd userAgentSwitcher
~$ pip install -r requirements.txt
[follow the example below for runtime usage]
```
## Example:

```
~$ python switcher.py https://jakereynolds.co -v -o output.txt
~$ cat output.txt
Trying user-agent: Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/54.0.2840.99 Safari/537.36
Trying user-agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/54.0.2840.99 Safari/537.36
Trying user-agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/54.0.2840.99 Safari/537.36
[TRUNCATED]
Comparing results
No differences found on https://jakereynolds.co
```



This tool is created for Ethical Hacking purposes, any illicit use is not related to its creator.

Currently undergoing development