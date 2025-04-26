### Create deployment dry run on client side

```aiignore
oc create deployment my-deployment -o yaml --image=bitnami/nginx  --dry-run=client > my-deplyment.yaml
```

### Create deployment dry run on server but not executing

```aiignore
oc apply -f my-deplyment.yaml --dry-run=server
```

### Create deployment dry run on server and validate

```aiignore
oc apply -f my-deplyment.yaml --dry-run=server --validate=true
```