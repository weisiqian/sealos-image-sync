将 ghcr.io 的镜像同步到 docker.io

支持同时同步多个镜像，每个镜像使用，分隔

示例：
```
sealos-cloud-terminal-frontend:latest,sealos-cloud-template-frontend:latest
```

镜像名称列表：

| 镜像 | 最新版 |
|---|---|
| sealos-cloud-terminal-frontend | sealos-cloud-terminal-frontend:latest | 
| sealos-cloud-template-frontend | sealos-cloud-template-frontend:latest | 
| sealos-cloud-desktop-frontend | sealos-cloud-desktop-frontend:latest | 
| sealos-cloud-applaunchpad-frontend | sealos-cloud-applaunchpad-frontend:latest | 
| sealos-cloud-costcenter-frontend | sealos-cloud-costcenter-frontend:latest | 
| sealos-cloud-license-frontend | sealos-cloud-license-frontend:latest | 
| sealos-cloud-dbprovider-frontend | sealos-cloud-dbprovider-frontend:latest | 
| sealos-cloud-cronjob-frontend | sealos-cloud-cronjob-frontend:latest | 
| sealos-cloud-adminer-frontend | sealos-cloud-adminer-frontend:latest | 
| sealos-cloud-terminal-controller | sealos-cloud-terminal-controller:latest | 
| sealos-cloud-user-controller | sealos-cloud-user-controller:latest | 
| sealos-cloud-app-controller | sealos-cloud-app-controller:latest | 
| sealos-cloud-license-controller | sealos-cloud-license-controller:latest | 
| sealos-cloud-resources-controller | sealos-cloud-resources-controller:latest | 
| sealos-cloud-database-service | sealos-cloud-database-service:latest | 
| sealos-cloud-account-controller | sealos-cloud-account-controller:latest | 
| sealos-cloud-job-init-controller | sealos-cloud-job-init-controller:latest | 
| sealos-cloud-job-heartbeat-controller | sealos-cloud-job-heartbeat-controller:latest | 
| sealos-cloud-objectstorage-controller | sealos-cloud-objectstorage-controller:latest | 
| sealos-cloud-node-controller | sealos-cloud-node-controller:latest | 
| sealos-cloud-db-adminer-controller | sealos-cloud-db-adminer-controller:latest | 
| sealos-cloud-account-service | sealos-cloud-account-service:latest | 
| sealos-cloud-admission-controller | sealos-cloud-admission-controller:latest | 
| sealos-cloud-pay-service | sealos-cloud-pay-service:latest | 
| sealos-cloud-minio-service | sealos-cloud-minio-service:latest | 
| sealos-applaunchpad-frontend | sealos-applaunchpad-frontend:latest | 
| sealos-desktop-frontend | sealos-desktop-frontend:latest | 
| sealos-cronjob-frontend | sealos-cronjob-frontend:latest | 
| sealos-terminal-frontend | sealos-terminal-frontend:latest | 
| sealos-costcenter-frontend | sealos-costcenter-frontend:latest |
| sealos-terminal-frontend | sealos-terminal-frontend:latest | 
| sealos-adminer-frontend | sealos-adminer-frontend:latest | 
| sealos-license-frontend | sealos-license-frontend:latest | 
| sealos-template-frontend | sealos-template-frontend:latest | 
| sealos-cloud | sealos-cloud:latest | 
| sealos-admission-controller | sealos-admission-controller:latest | 
| sealos-app-controller | sealos-app-controller:latest | 
| sealos-account-controller | sealos-account-controller:latest | 
| sealos-job-heartbeat-controller | sealos-job-heartbeat-controller:latest | 
| sealos-license-controller | sealos-license-controller:latest | 
| sealos-db-adminer-controller | sealos-db-adminer-controller:latest | 
| sealos-job-init-controller | sealos-job-init-controller:latest | 
| sealos-resources-controller | sealos-resources-controller:latest | 
| sealos-account-service | sealos-account-service:latest | 
| sealos-objectstorage-controller | sealos-objectstorage-controller:latest | 
| sealos-node-controller | sealos-node-controller:latest | 
| sealos-terminal-controller | sealos-terminal-controller:latest | 
| sealos-database-service | sealos-database-service:latest | 
| sealos-minio-service | sealos-minio-service:latest | 
| sealos-user-controller | sealos-user-controller:latest | 
| sealos-pay-service | sealos-pay-service:latest | 
| sealos-objectstorage-frontend | sealos-objectstorage-frontend:latest |

最新版镜像

```
sealos-cloud-terminal-frontend:latest,sealos-cloud-template-frontend:latest,sealos-cloud-desktop-frontend:latest,sealos-cloud-license-frontend:latest,sealos-cloud-applaunchpad-frontend:latest,sealos-cloud-dbprovider-frontend:latest,sealos-cloud-cronjob-frontend:latest,sealos-cloud-costcenter-frontend:latest,sealos-cloud-adminer-frontend:latest,sealos-cloud-app-controller:latest,sealos-cloud-terminal-controller:latest,sealos-cloud-user-controller:latest,sealos-cloud-job-init-controller:latest,sealos-cloud-database-service:latest,sealos-cloud-job-heartbeat-controller:latest,sealos-cloud-license-controller:latest,sealos-cloud-resources-controller:latest,sealos-cloud-account-controller:latest,sealos-cloud-objectstorage-controller:latest,sealos-cloud-node-controller:latest,sealos-cloud-db-adminer-controller:latest,sealos-cloud-account-service:latest,sealos-cloud-pay-service:latest,sealos-cloud-admission-controller:latest,sealos-cloud-minio-service:latest,sealos-desktop-frontend:latest,sealos-cronjob-frontend:latest,sealos-applaunchpad-frontend:latest,sealos-costcenter-frontend:latest,sealos-dbprovider-frontend:latest,sealos-dbprovider-frontend:latest,sealos-adminer-frontend:latest,sealos-template-frontend:latest,sealos-license-frontend:latest,sealos-cloud:latest,sealos-job-heartbeat-controller:latest,sealos-job-init-controller:latest,sealos-resources-controller:latest,sealos-db-adminer-controller:latest,sealos-admission-controller:latest,sealos-app-controller:latest,sealos-account-controller:latest,sealos-license-controller:latest,sealos-objectstorage-controller:latest,sealos-account-service:latest,sealos-user-controller:latest,sealos-node-controller:latest,sealos-terminal-controller:latest,sealos-database-service:latest,sealos-minio-service:latest,sealos-pay-service:latest,sealos-objectstorage-frontend:latest
```

工具JS

解析所有镜像的名称和标签

```
# https://github.com/weisiqian?page=2&tab=packages

Array.from(document.querySelectorAll(".flex-auto>a")).map(item => `${item.innerText}:latest`).join(',')
```

生成指定标签的镜像名称
```js
[
  "sealos-cloud-terminal-frontend",
  "sealos-cloud-template-frontend",
  "sealos-cloud-cronjob-frontend",
  "sealos-cloud-desktop-frontend",
  "sealos-cloud-applaunchpad-frontend",
  "sealos-cloud-license-frontend",
  "sealos-cloud-dbprovider-frontend",
  "sealos-cloud-costcenter-frontend",
  "sealos-cloud-adminer-frontend",
  "sealos-cloud-app-controller",
  "sealos-cloud-terminal-controller",
  "sealos-cloud-user-controller",
  "sealos-cloud-database-service",
  "sealos-cloud-job-heartbeat-controller",
  "sealos-cloud-resources-controller",
  "sealos-cloud-job-init-controller",
  "sealos-cloud-account-controller",
  "sealos-cloud-license-controller",
  "sealos-cloud-db-adminer-controller",
  "sealos-cloud-pay-service",
  "sealos-cloud-objectstorage-controller",
  "sealos-cloud-node-controller",
  "sealos-cloud-account-service",
  "sealos-cloud-minio-service",
  "sealos-cloud-admission-controller",
  "sealos-dbprovider-frontend",
  "sealos-applaunchpad-frontend",
  "sealos-costcenter-frontend",
  "sealos-desktop-frontend",
  "sealos-cronjob-frontend",
  "sealos-desktop-frontend",
  "sealos-cronjob-frontend",
  "sealos-terminal-frontend",
  "sealos-license-frontend",
  "sealos-cloud",
  "sealos-job-heartbeat-controller",
  "sealos-job-init-controller",
  "sealos-resources-controller",
  "sealos-db-adminer-controller",
  "sealos-admission-controller",
  "sealos-app-controller",
  "sealos-account-controller",
  "sealos-license-controller",
  "sealos-objectstorage-controller",
  "sealos-account-service",
  "sealos-user-controller",
  "sealos-node-controller",
  "sealos-terminal-controller",
  "sealos-database-service",
  "sealos-minio-service",
  "sealos-pay-service",
  "sealos-objectstorage-frontend"
].map(item => `${item}:latest`).join(',')
```