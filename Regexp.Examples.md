## Regexp Examples
----------------------------------------------------------------------------------------------

localhost
localhost:3000

some.domail.local
some.domail.local:80
some.domail.local:8080

anoth-er.cool-domain
anoth-er.cool-domain:80
anoth-er.cool-domain:8000

antés-lãrech.com # <= the new domains to come...
antés-lãrech.com:22
antés-lãrech.com:3333

1.2.3.4
1.2.3.4:1
1.2.3.4:12
1.2.3.4:123
1.2.3.4:1234

127.0.0.1
127.0.0.1:80
127.0.0.1:1234
192.168.1.330
192.168.1.330:80
192.168.1.330:1234

http://192.168.1.330:1234/
http://192.168.1.330:1234:80/
http://192.168.1.330:1234:8080/

----------------------------------------------------------------------------------------------

#### TODOs:
* 1) Parse for this => http://192.168.1.330:1234:8080/app/users/supermind/cool/function?and=0&some=query&here=and&there=213553
* 2) Replace normal matchers to return named-matchers like this <:prococol><:local|tts><:subdomains><:domain><:port><:path><:params><:anchor><:whatelse>

----------------------------------------------------------------------------------------------

#### Use Regex (Regular Expressions) to find IPv4 on files
##### Run this regexp finder:
* ```((http|ftp|ssh|git)):\/\/)*(([0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3})|localhost|[\w\W]*)(\:[0-9]{1,9})*```

#### Use this "Replacer" and see the result like this:
* ```$1 - 2: $2 - 3: $3 - 4: $4 - 5: $5 - 6: $6 - 7: $7 - 8: $8 - 9: $9 - 10: $10 - 11: $11```

----------------------------------------------------------------------------------------------

#### [1] TODO:
* Test. These regexp is not yet working 100% as needed (v120527-a01.03a)
