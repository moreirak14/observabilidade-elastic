# You want to use elasticsearch beats? Let's go...

# - Have you tried using metricbeat and nothing worked??
1º view the metricbeat logs with this command: docker logs metricbeat or docker logs heartbeat

# The logs returned the error below? Please follow the next steps:

# Error
# metricbeat or heartbeat:
1) - Exiting: error loading config file: config file ("metricbeat.yml") can only be writable by the owner but the permissions are "-rw-rw-r--" (to fix the permissions use: 'chmod go-w /usr/share/metricbeat/metricbeat.yml')

# Results
# metricbeat or heartbeat:
1) - sudo chown root metricbeat.yml and sudo chmod 0644 metricbeat.yml
