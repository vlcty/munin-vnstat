munin-vnstat
============

A munin plugin to visualize daily traffic stats.
The plugin draws three graphs: Inbound, outbound and overall traffic based on data collected by ``vnstat``.
It's normal that the graphs drop to 0 after 24 o'clock because the counters a reset to 0.

Installation
------------

Checkout this repository to ``/usr/share/munin/plugins``. Afterwards you have to create a softlink:

``ln -s /usr/share/munin/plugins/munin-vnstat/vnstat_ /etc/munin/plugins/vnstat_etho``, in order to monitor eth0.

The plugin has autoconf and suggest capabilities, so you can do:
``munin-node-configure --shell --libdir=/usr/share/munin/plugins/munin-vnstat/ | bash``, in order to automatically
create the links.

After a few runs you can already see the output.
After a day you can see a nice drawing.
After a week you can see your peak time.
