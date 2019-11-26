# kubernetes-resource

A Kubernetes Concourse resource

## Installing

```
resource_types:
  - name: kubernetes
    type: docker-image
    source:
      repository: thefoxjob/concourse-kubernetes-resource
resources:
  - name: kubernetes
    type: kubernetes
    source:
      server: ((k8s_server_url))
      namespace: default
      token: ((k8s_bearer_token))
```

#### `out`: Begins Kubernetes deploy process
