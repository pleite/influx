# influx

Kubernetes deployment to carry a telegraf container as a DaemonSet and provide stats to Influx CloudDB 2.0 Beta

Please create the required secrets from the CloudDB interface:

kubectl create secret -n monitoring generic telegraf --from-literal=influx_token=*mime base64* --from-literal=influx_config=https://us-west-2-1.aws.cloud2.influxdata.com/api/v2/telegrafs/ *your id from the configuration*

