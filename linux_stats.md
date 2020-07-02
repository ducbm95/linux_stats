## Traffic
dstat -n -N wlp3s0,tun0

## CPU (%user %nice %system %idle)
iostat
top -n 1
top -b -n 1
dstat -c

## Load CPU (1m 5m 15m)
top -n 1
top -b -n 1
dstat -l

## Memory/Swap (total used free cache)
free -m
top -n 1
top -b -n 1
dstat -m

## TCP Stats

## Disk Usage
df -h

## Disk Statistics
### Disk Read/Write (Mb/s) (Read | Write)
dstat -d -D nvme0n1p1 60

### Disk Request/s (MergedRead | MergedWrite | Read | Write)
dstat --disk-tps -D nvme0n1p1 60

### Disk Time (ServiceTime | AWait)
dstat -D nvme0n1p1 --disk-svctm 60 # ServiceTime
dstat -D nvme0n1p1 --disk-wait

### Disk Utilization
dstat -D sdb --disk-util 60

### Disk RequestSize
dstat -D nvme0n1p1 --disk-avgrq 60

### Disk QueueSize
dstat -D nvme0n1p1 --disk-avgqu 60

## Each process
### Memory
top -n 1
top -b -n 1

### CPU
top -n 1
top -b -n 1

## Common
All stats will have (max | avg | current) value.
dstat
