## grafana helm-values.yaml
```
dashboardProviders:
  dashboardproviders.yaml:
    apiVersion: 1
    providers:
    - name: '<provider_name>'
      orgId: 1
      folder: '<folder>'
      type: file
      disableDeletion: true
      editable: true
      options:
        path: /var/lib/grafana/dashboards/<provider_name>
```
```
dashboards: 
  <provider_name>:
    <dashboard_name>:  
      url: https://raw.githubusercontent.com/nasmolin/grafana_dashboards/refs/heads/main/loki-unique-value-counter.json
```
___
## loki-unique-value-counter.json
<img src="/resources/loki-unique-string-counter.png" alt="loki-unique-string-counter" width="700"/>



