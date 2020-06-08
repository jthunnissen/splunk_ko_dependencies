# Splunk knowledge objects_dependencies
A splunk app for app developers to search and investigate dependencies between knowledge objects

version support: Splunk Enterprise 7+

## installation
In stall the Splunk and on your searchhead as normal.

One special requirement of the app is it requires liberal limits on regular expression processing. If these are not in place large knowledge objects, such as big dashboards, will not be fully parsed for dependencies. The app comes distributed with the following limits.conf, which should be sufficient for most environments.

```
INSERT
```

Make sure to not override these limits in hour system local configuration.
