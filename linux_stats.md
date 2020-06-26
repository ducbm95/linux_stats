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
dstat ??

### Disk Request/s (MergedRead | MergedWrite | Read | Write)
dstat ??

### Disk Time (ServiceTime | AWait)
dstat ??

### Disk Utilization
dstat ??

### Disk RequestSize
dstat ??

### Disk QueueSize
dstat ??

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
