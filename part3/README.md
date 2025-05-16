Delete the database that was being used before by using:

```
kubectl delete deploy products-db
kubectl delete svc products-db
kubectl delete pvc -l app=products-db
```
Deploy the changes using:
```
kubectl apply -f < name-of-the-file >.yaml
```

