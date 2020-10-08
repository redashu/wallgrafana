# Graphine in an Image

<img src="gin.png">

## More easier way to deploy graphite will be container model 

<img src="gdocker.png">

## stopping graphite related services

<img src="grastop.png">


## pulling docker image for graphite and statsD

<img src="statsdocker.png">

## starting container 

```
sudo docker run --name graphite-statsd  -itd  --restart always  -p 80:80 -p 8125:8125/udp -p 8126:8126 -p 2003-2004:2003-2004 -p 2023-2
024:2023-2024   graphiteapp/graphite-statsd

```

## sending data to carbon using bash / sh 

```
 echo  "stats.ubuntu.tmp.file.count 10 `date +%s`" |  nc  -w0  localhost 2003
```

## sending data to statsD using bash on UDP 

<img src="datastats.png">

