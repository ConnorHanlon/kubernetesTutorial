# kubernetesTutorial

## Starting nginx
```
cd c:\
cd nginx
start nginx
```

### nginx commands
```
nginx -s stop	fast shutdown
nginx -s quit	graceful shutdown
nginx -s reload	changing configuration, starting new worker processes with a new configuration, graceful shutdown of old worker processes
nginx -s reopen	re-opening log files
```

### nginx more info
http://nginx.org/en/docs/windows.html

By default nginx listens on port 80- localhost:80


### Starting the sa-webapp with Spark/Java
```
cd sa-webapp
```

if no target directory:
```
mvn install
```

Next:
```
cd target
java -jar sentiment-analysis-web-0.0.1-SNAPSHOT.jar --sa.logic.api.url=http://localhost:5000
```

### Starting SA logic with Flask/Python

```
cd sa-logic/sa
python sentiment_analysis.py
```

### Stopping SA Logic and SA-Webapp Servers
ctrl-c
