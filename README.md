# cngo v1
> **Fast Golang Tool take a filename with domains and get cname for every domain**


![Image of Cngo](https://i.imgur.com/zQ6cMYF.gif)

# Install
```
$ go get -u github.com/yghonem14/cngo
```

## Basic Usage
cngo accepts only text files:

```
$ cngo -f ~/targets/spotify.txt
creativeservice.spotify.com -> creativeservicespotify.s3.amazonaws.com
crashdump.spotify.com -> www.crashdump.s3.amazonaws.com
```


## Concurrency

You can set the concurrency value with the `-c` flag:

```
$ cngo -f ~/targets/spotify.txt -c 35
```

## Timeout

You can set the timeout by using the `-t`:

```
$ cngo -f ~/targets/spotify.txt -t 3
```
