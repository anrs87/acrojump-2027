# Deploy en Netlify — ACROJUMP

Desde PowerShell en esta carpeta (`f:\Proyectos\AGENTE PERSONAL\tools\landing_acrojump`), usá `npx.cmd` (en esta PC PowerShell bloquea `npx.ps1`):

1. Iniciar sesión (una sola vez):
```powershell
npx.cmd netlify-cli login
```

2. Publicar en producción:
```powershell
npx.cmd netlify-cli deploy --dir . --prod
```

- La configuración de publicación (`publish = "."`) y la caché de `/assets/*` ya están definidas en `netlify.toml`.
- Si es la primera vez que deployás la carpeta, `netlify-cli` te va a pedir crear o vincular un sitio en tu cuenta.
