# Роли и их полномочия при работе с Kubernetes

| Роль  | Права роли | Группы пользователей |
| --- | --- | --- |
|viewer|	ClusterRole — доступ только к чтению всех ресурсов и компонентов|Аналитики, QA, ИБ, мониторинг|
|editor|	Role — создание и редактирование ресурсов в namespace, без secrets|Разработчики|
|admin|Role — полный доступ в namespace, включая secrets, ingress и volume|DevOps, старшие разработчики, SRE|
|secrets-reader|Role — доступ только на чтение secrets в нужных namespace|Служба ИБ, DLP, аудит|
|cluster-admin|ClusterRole (встроенная) — полный контроль над кластером|Kubernetes-админы, главный DevOps |
