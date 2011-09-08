# total-uptime 

<http://github.com/dbb/total-uptime>

## Description
**total-uptime** is a wrapper for commands that involve turning your computer 
off, like `shutdown` and `pm-hibernate`. In addition to running the desired 
command, **total-uptime** also parses the data from the `uptime` utility to 
find out how long the machine has been running, and it saves this data in a 
local log file. Every time the command is called, it adds the previous data
to the current data. This allows you to keep a running total of your uptime.

However, this approach fails in the event that the machine is shut off 
unexpectedly, as in the event of a power outage. Thus, **total-uptime** can 
be run as a daemon and update the uptime data in a defined interval (the 
default is one hour). This behavior is optional.

