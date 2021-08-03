---
title: Engine supported Time Zones
authors: mbetak, sabusale
---

# Engine supported Time Zones

Engine default time-zones can be found in <ENGINE_DEPLOYMENT>/etc/ovirt-engine/timezones/00-defaults.properties

####Timezones file format:

key must be valid timezone from tz database, value must be valid windows timezone

for example, see [here](https://github.com/oVirt/ovirt-engine/blob/master/packaging/conf/timezones-defaults.properties#L12)


## Extending the time zone list:
ovirt users can extend the default time zone list and add their own timezones

In order to do that:
- add new file in <ENGINE_DEPLOYMENT>/etc/ovirt-engine/timezones, for example: 10-timezones.properties
- add your own time zone with correct format (see above for more)
- restart the engine

After following this steps new time zone should appear on the engine and can be used