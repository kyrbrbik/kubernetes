install with helm

helm upgrade prometheus prometheus-community/kube-prometheus-stack -f values.yml

patch grafana dashboard

kubectl patch cm grafana-config-dashboards --patch-file patch-grafana-config-dashboards.yml
