# Запуск и проверка RBAC

1. Инициализируем minikube.
```bash
minikube start
```
2. Создаем пользователей.
```bash
chmod +x create-users.sh
./create-users.sh
```
3. Применяем RBAC-роли: (roles.yaml)
```bash
kubectl apply -f roles.yaml
```
4. Настраиваем привязки ролей: (rolebinding.yaml)
```
kubectl apply -f rolebindings.yaml
```
