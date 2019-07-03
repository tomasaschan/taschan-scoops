# taschan-scoops

A [scoop.sh](https://scoop.sh) bucket with stuff I've needed, but not wanted to trust unknown buckets with.

## Setup scoop

```powershell
Set-ExecutionPolicy RemoteSigned -s cu -force
iex (new-object net.webclient).downloadstring('https://get.scoop.sh')
scoop install git
scoop bucket known | % { scoop bucket add \$\_ }
scoop update
```

## Add this bucket

```powershell
scoop bucket add tomasaschan https://github.com/tomasaschan/taschan-scoops
```
