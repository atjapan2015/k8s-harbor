
```
helm install my-release --set externalURL=https://core.harbor.k8scloud.site --set expose.ingress.hosts.core=core.harbor.k8scloud.site --set expose.ingress.hosts.notary=notary.harbor.k8scloud.site  --set persistence.persistentVolumeClaim.jobservice.storageClass=local-path --set persistence.persistentVolumeClaim.registry.storageClass=local-path --set persistence.persistentVolumeClaim.chartmuseum.storageClass=local-path --set persistence.persistentVolumeClaim.redis.storageClass=local-path --set persistence.persistentVolumeClaim.database.storageClass=local-path --namespace public-service harbor/harbor
```

# helm
```
 Install harbor to k8s by helm: https://www.cnblogs.com/dukuan/p/9963744.html
 Install redmine to k8s by helm: https://www.cnblogs.com/dukuan/p/10020266.html
 Install jenkins to k8s by helm: https://www.cnblogs.com/dukuan/p/10020266.html
```
