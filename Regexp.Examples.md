## Regexp Examples
### Use in Sublime Text 2

localhost
localhost:3000

some.domail.local
some.domail.local:80
some.domail.local:8080

anoth-er.cool-domain
anoth-er.cool-domain:80
anoth-er.cool-domain:8000

###### the new domains to come (with accents and -maybe- ascii caracters too)
antés-lãrech.com
antés-lãrech.com:22
antés-lãrech.com:3333

1.2.3.4
1.2.3.4:80
1.2.3.4:123
1.2.3.4:1234

127.0.0.1
127.0.0.1:80
127.0.0.1:1234

http://192.168.1.330/
https://192.168.1.330:1234/

ftp://192.168.1.330:1234/
ssh://192.168.1.330:1234/
git://192.168.1.330:1234/

https://192.168.1.330:8080/app/users/supermind/cool/function?and=0&some=query&here=and&there=213553

----------------------------------------------------------------------------------------------

#### TODOs:
* 1) Parse for this => ```http://192.168.1.330:1234:8080/app/users/supermind/cool/function?and=0&some=query&here=and&there=213553```
* 2) Replace normal matchers to return named-matchers like this ```<:prococol><:local|tts><:subdomains><:domain><:port><:path><:params><:anchor><:whatelse>```
* 3) Improve this regex

----------------------------------------------------------------------------------------------

#### Working example

#### Use Regex (Regular Expressions) to find IPv4 on files/scripts

##### Run this regexp finder:
* ```(?<protocol>[http|https|ftp|ssh|git\:\/\/]?)*(?<domain>[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}|[a-Z0-9\-\_\.]?)*(?<port>[\:0-9]{1,9}?)*(?<url>[a-Z0-9\/\-\_\.]?)*(?<query>[a-Z0-9\=\&\%\#\?\/\-\_\.]?)*```

#### Use this "replacer" and see the results (use/test it to understand the results):
* ```$0 --- $1 --- $2 --- $3 --- $4 --- $5 --- $6 --- $7 --- $8```

----------------------------------------------------------------------------------------------

#### [1] TODO:
* How use named regex be used to show results in Sublime Text ?
