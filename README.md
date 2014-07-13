KONACli
=======

KONA Command Line Tool


# Download the latest

https://github.com/konacloud/KONACli/raw/master/releases/kcli.zip
# Demo Video

https://konacloud2.wistia.com/medias/1oh4dvjjt6

# Add an alias

after download make and alias to 'sh kona.sh' like this

```
alias kona='sh /Users/santiago/kona/kona.sh'
```

To add the alias permanent, just add here

```
nano ~/.bash_profile
```

we asume that you hace the alias kona

# Login

Only need to login one time

```
santiagos-mbp:kona santiago$ kona --login
Enter your userId: taio
Enter your secret password: 
{"success":true}
Login success!!
santiagos-mbp:kona santiago$ 
```

# Apps

List my apps

```
santiagos-mbp:kona santiago$ kona --apps
0 - ticket
1 - searchTest
2 - samples
3 - demo
4 - TramitesUY
5 - penca
6 - tbpm
7 - hello
8 - CookerApp
santiagos-mbp:kona santiago$ 
```
# Download app

```
santiagos-mbp:kona santiago$ kona --download hello
Downloading file...please wait
Temp file created /Users/santiago/kona/taio/hello/1405212245981.zip
Extracting file...please wait
file created : /Users/santiago/kona/taio/hello/readme
file created : /Users/santiago/kona/taio/hello/apis/timeUtil.js
file created : /Users/santiago/kona/taio/hello/libs/timeUtil.js
file created : /Users/santiago/kona/taio/hello/apis/api.js
file created : /Users/santiago/kona/taio/hello/models/Person.js
file created : /Users/santiago/kona/taio/hello/apis/asdf.js
file created : /Users/santiago/kona/taio/hello/apis/rr.js
Removing temp file ?true
Done
santiagos-mbp:kona santiago$ 
```

# Push app

```
santiagos-mbp:kona santiago$ kona --push hello
file found/Users/santiago/kona/taio/hello/models/Person.js
file found/Users/santiago/kona/taio/hello/apis/api.js
file found/Users/santiago/kona/taio/hello/apis/asdf.js
file found/Users/santiago/kona/taio/hello/apis/rr.js
file found/Users/santiago/kona/taio/hello/apis/timeUtil.js
push all this? y/n y
-> Push file Person.js
--> Resource Id mr_Person
--> Resource Content /Users/santiago/kona/taio/hello/models/Person.js
{"success":true}
-> Push file api.js
--> Resource Id r_api
--> Resource Content /Users/santiago/kona/taio/hello/apis/api.js
{"success":true}
-> Push file asdf.js
--> Resource Id r_asdf
--> Resource Content /Users/santiago/kona/taio/hello/apis/asdf.js
{"success":true}
-> Push file rr.js
--> Resource Id r_rr
--> Resource Content /Users/santiago/kona/taio/hello/apis/rr.js
{"success":true}
-> Push file timeUtil.js
--> Resource Id r_timeUtil
--> Resource Content /Users/santiago/kona/taio/hello/apis/timeUtil.js
{"success":true}
santiagos-mbp:kona santiago$ 
```

# Help

```
santiagos-mbp:kona santiago$ kona --help
[ option: help  :: help ]
[ option: download  [ARG] :: download one app ]
[ option: login  :: login into konacloud ]
[ option: push  [ARG] :: push one app ]
[ option: apps  :: list apps ]
santiagos-mbp:kona santiago$ 
```
