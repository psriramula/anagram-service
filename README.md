# anagram-service

Play Framework based anagram-service to implement an anagram-service

The task

You need to put together a simple web application that can produce anagrams of words from a wordlit.

·  You can find a copy of our wordlist at http://static.abscond.org/wordlist.txt
·  Non-alphanumeric characters should be considered as part of the anagram (e.g. "he's" is not an anagram of "she")
·  The application should be able to respond to a request made every second
·  Assume that the application will be hosted on heroku
Details

The application should be able to receive an HTTP GET request with the requested word as the path. It should return the results as JSON. See the example below:

GET /crepitus
{"crepitus":["cuprites","pictures","piecrust"]}


GET /crepitus,paste,kinship,enlist,boaster,fresher,sinks,knits,sort
{"crepitus":["cuprites","pictures","piecrust"],"paste":["pates","peats","septa","spate","tapes","tepas"],"kinship":["pinkish"],"enlist":["elints","inlets","listen","silent","tinsel"],"boaster":["boaters","borates","rebatos","sorbate"],"fresher":["refresh"],"sinks":["skins"],"knits":["skint","stink","tinks"],"sort":["orts","rots","stor","tors"]}


GET /sdfwehrtgegfg
{"sdfwehrtgegfg":[]}

Requirements
-------------------------

Required following tools to build and run this application
1. JDK 1.8
2. sbt 0.13 to - for compiling, testing, packaging and running.

Development environment setup
-------
Its a sbt based project intended to compile and run for  JDK 1.8 X. You can import this as a sbt project in to your IDE ( Eclipse or IntelliJ) as
standard sbt project and able to browse and start development.

Testing
-------
To run the Unit Tests included with in the application, change to application folder

```
$ sbt test
```

Running
-------

To run the applicaton to with generate daily cost per user for the calls.log file with in the resources

```
$ sbt run
```



## Project Template Source
- Project template taken from https://github.com/playframework/play-scala-starter-example/tree/2.6.x and may have references
