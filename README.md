
```
https://github.com/goharbor/harbor-helm
```

```
helm install harbor --set externalURL=https://core.harbor.k8scloud.site --set expose.ingress.hosts.core=core.harbor.k8scloud.site --set expose.ingress.hosts.notary=notary.harbor.k8scloud.site --set persistence.persistentVolumeClaim.jobservice.storageClass=local-path --set persistence.persistentVolumeClaim.registry.storageClass=local-path --set persistence.persistentVolumeClaim.chartmuseum.storageClass=local-path --set persistence.persistentVolumeClaim.redis.storageClass=local-path --set persistence.persistentVolumeClaim.database.storageClass=local-path --set persistence.persistentVolumeClaim.registry.size=20Gi --namespace public-service harbor/harbor
```

Edit svc
```
core.nodePort: 31903
notary-server.nodePort: 31953
portal.nodePort: 32597
```

# helm
```
 Install harbor to k8s by helm: https://www.cnblogs.com/dukuan/p/9963744.html
 Install redmine to k8s by helm: https://www.cnblogs.com/dukuan/p/10020266.html
 Install jenkins to k8s by helm: https://www.cnblogs.com/dukuan/p/10020266.html
```
