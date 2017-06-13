============= === ======= ======= ========== ======= === ============ =========
Component     HA  Scaling Logging Monitoring Ingress PV  LoadBalancer Grafana
                                                                      Dashboard
============= === ======= ======= ========== ======= === ============ =========
cassandra     yes yes     yes     yes        no      yes no
elasticsearch yes yes     N/A     no         yes     yes yes
elk-cluster   N/A N/A     N/A     no         N/A     N/A N/A
grafana       no  ?       no      N/A        yes     yes yes
hdfs          yes no      no      no         yes     yes yes
iot-gen       N/A N/A     N/A     N/A        N/A     N/A N/A
kafka         yes yes     yes     yes        N/A     yes no
kibana        yes yes     N/A     no         yes     N/A yes
logstash      yes yes     N/A     no         N/A     N/A no
mariadb       no  no      yes     yes        N/A     yes yes
mongodb       yes yes     no      no         N/A     no  yes
postgresql    no  no      no      yes        N/A     yes yes
prometheus    yes yes     no      N/A        yes     yes yes
rabbitmq      yes yes     no      yes        yes     yes yes
redis         yes yes     no      no         N/A     yes no
spark         yes yes     yes     yes        yes     N/A yes
tweepub       N/A N/A     N/A     N/A        N/A     N/A N/A
tweetics      N/A N/A     N/A     N/A        N/A     N/A N/A
tweeviz       N/A N/A     N/A     N/A        N/A     N/A N/A
zookeeper     yes yes     no      yes        N/A     yes no
============= === ======= ======= ========== ======= === ============ =========
