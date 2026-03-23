# appprueba2

appPrueba2

**Proyecto:** bup-policies-pro
**Lenguaje:** python
**Puerto:** 8080

## Desarrollo local

```bash
# Go
go run .

# Python
python main.py

# Node.js
node index.js
```

## Build y push de imagen

```bash
# Build
docker build -t registry.local:5000/bup-policies-pro/appprueba2:latest .

# Push al registro interno de Kind
docker push registry.local:5000/bup-policies-pro/appprueba2:latest
```

## Acceso

Una vez desplegado en el cluster:

```
http://appprueba2.bup-policies-pro.local
```

Agregar al `/etc/hosts`:
```
127.0.0.1  appprueba2.bup-policies-pro.local
```

## GitOps

Los manifiestos Kubernetes están en:
```
https://github.com/NicoMiretti/idp-local/tree/main/gitops/platform/bup-policies-pro/base/apps/appprueba2
```
