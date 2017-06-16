The f scripts load Bitnami's Hadoop and Hbase, then set about trying to run Geowave.

Here are a few manual workarounds:
* add to walnut.sh INSTALL_DIR=/tmp/geowave
* s/GEOWAVE_VERSION=0.9.5/0.9.4/ in walnut.sh?
* one of the f# modules needed updating the version number because right away the wget was failing
* geowave-env.sh has 0.9.5 hardcoded so I changed it to 0.9.4
* /tmp/geowave/ in line 41

Even with the manual workarounds, Geowave isn't running.

I'm not taking the time to find the glitch, as I'm not actively working with Geowave.

I'm preserving the scripts mostly in case there are some interesting script tricks.

I also have notes about using Hortonworks instead of Bitnami, stored offline and not in a repo, from around May 2017.
