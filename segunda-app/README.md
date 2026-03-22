# segunda-app

App para testear catalog register

**Proyecto:** test-proyecto
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
docker build -t registry.local/test-proyecto/segunda-app:latest .

# Push al registro interno de Kind
docker push registry.local/test-proyecto/segunda-app:latest
```

## Acceso

Una vez desplegado en el cluster:

```
http://segunda-app.test-proyecto.local
```

Agregar al `/etc/hosts`:
```
127.0.0.1  segunda-app.test-proyecto.local
```

## GitOps

Los manifiestos Kubernetes están en:
```
https://github.com/NicoMiretti/idp-local/tree/main/gitops/platform/test-proyecto/base/apps/segunda-app
```
