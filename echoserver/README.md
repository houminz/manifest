# http-echo

HTTP Echo is a small go web server that serves the contents it was started with
as an HTML page.

The default port is 5678, but this is configurable via the `-listen` flag:

```
http-echo -listen=:8080 -text="hello world"
```

Then visit http://localhost:8080/ in your browser.


```
$ docker run -p 8080:8080 hashicorp/http-echo -listen=:8080 -text="hello world" -d
flag provided but not defined: -d
Usage of /http-echo:
  -listen string
    	address and port to listen (default ":5678")
  -text string
    	text to put on the webpage
  -version
    	display version information
```

see [github](https://github.com/hashicorp/http-echo)
