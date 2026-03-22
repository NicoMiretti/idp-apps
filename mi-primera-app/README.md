# mi-primera-app

Primera app de prueba

**Proyecto:** test-proyecto
**Lenguaje:** go
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
docker build -t registry.local/test-proyecto/mi-primera-app:latest .

# Push al registro interno de Kind
docker push registry.local/test-proyecto/mi-primera-app:latest
```

## Acceso

Una vez desplegado en el cluster:

```
http://mi-primera-app.test-proyecto.local
```

Agregar al `/etc/hosts`:
```
127.0.0.1  mi-primera-app.test-proyecto.local
```

## GitOps

Los manifiestos Kubernetes están en:
```
https://github.com/NicoMiretti/idp-local/tree/main/gitops/platform/test-proyecto/base/apps/mi-primera-app
```
