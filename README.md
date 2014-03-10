munin-vnstat
============

Plugin for munin to display the network traffic for the current day

The plugin displays the daily traffic in megabytes.
The red graph shows the amount of incoming traffic and the green one the outgoing traffic.
The black graph just sums it up to have a better overview.

Requires a running vnstat daemon which updates the database.

Example
-------

This picture shows an example of an output:

![Example after a few houres running](http://files.veloc1ty.de/munin-examples/vnstat/vnstat1.png "vnStat Sample 1")


Installation
------------

Place vnstat in

/usr/share/munin/plugins

and link it with

ln -s /usr/share/munin/plugins/vnstat /etc/munin/plugins/vnstat