# Containers dicas

## HELM

```
helm show values name/name > values_name.yaml
helm install name name/name -f values-name.yaml --namespace name
helm install -f values-name.yaml --wait --namespace name --create-namespace name name/name
```

### Example

```
helm upgrade prometheus-server prometheus-community/prometheus -f values_prometheus.yaml -n monitoring
```
