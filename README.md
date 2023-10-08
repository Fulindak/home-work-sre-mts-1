# home-work-sre-mts-ansible-helm


---

## Схема кластера :

![image.png](img/image.png)

---
## Ansible  playbook

- Добавить свои хосты в файл invetory
- Настроить под себя файл vars/main.yml
#### Запуск деплоя:
```
ansible-playbook -i inventory deploy_pgcluster.yml
```
---
## Helm Chart

- Внести инфформацию о своем сервисе  в configmap.yaml
- Добавить свои эндпоинты и настроить deployment.yaml
- Изменить под себя variables, service.port, ingress и resources в  values.yaml

### Запуск helm chart:
```
helm install  weather-api weather-api --kubeconfig=kuberconfig.yaml
```

---
### Ссылка на репозиторий с postgresql-cluster : 
>https://github.com/vitabaks/postgresql_cluster.git
