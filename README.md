# Cobalt strike custom 404 page

## Note to upgrade to version 4.0:
At the moment, this update is in a test state. I need to understand a few fragments of code and conduct additional tests. But it seems that the update is already working, if you find an error in the code or run into problems let me know, I will try to fix it.  
As before, I used jdk 13 to compile, if you use a different version of java to work, you should compile yourself using the following command: `javac -classpath cobaltstrike.jar WebServer.java`
Many thanks to the author for the idea. Using Cobalt Strike it is worth avoiding as much as possible standard elements that can be noticeable from the outside.

## why use this?

You can find the CS service through 404 pages.

Just like:
```
https://www.zoomeye.org/searchResult?q=%22HTTP%2F1.1+404+Not+Found+++Content-Type%3A+text%2Fplain+Date%3A%22+%2B%22Content-Length%3A+0%22+-Connection
```

![Image](https://github.com/XZVB12/cs_custom_404/raw/master/img/2019-03-21-17-49-22.png)

So, we need custom 404.


## how to use?

Open cobaltstrike.jar with rar, and replace `cloudstrike\WebServer.class` with `WebServer.class`.

Then put a 404.html to `resources` folder。

## Test

![Image](https://github.com/XZVB12/cs_custom_404/raw/master/img/2019-03-21-17-55-42.png)
