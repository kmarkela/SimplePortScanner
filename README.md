# Simple TCP Port Scanner

### Params

```bash 
  -h string
        hosts, e.g. 172.16.1.1,172.16.1.2
  -p string
        ports, e.g. 80,22
  -t int
        TCP timeout (default 5)
  -v    Verbose
  -w int
        Workers (default 5)
```

### Build 

```bash
go build main.go -o bin/sps
OOS=windows GOARCH=amd64 go build -o bin/sps.exe
```

### Example
```
.\sps.exe -h 172.16.1.1,172.16.1.2 -p 80,81,8080 -t 2 -w 10 
```