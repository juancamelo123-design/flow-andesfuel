# Flow · Dashboard y agente de disputas

Prototipos de la prueba técnica de Periferia (caso Flow / AndesFuel). Todos los datos son ficticios.

| Ruta | Qué es |
|---|---|
| `index.html` | Dashboard por rol (Comité, Producto, Jefe de zona, Estación, Riesgo, Ingeniería), con filtro por estación, semana y resumen por correo del agente. |
| `agente/index.html` | Agente de disputas en vivo sobre la API de Claude: herramientas de solo lectura, reglas de seguridad en código y aprobación humana. |
| `assets/logo-flow.png` | Logo de Flow. |

## Publicar con GitHub Pages
1. Sube esta carpeta a un repositorio.
2. En **Settings → Pages**, elige la rama `main` y la carpeta `/ (root)`.
3. El dashboard queda en `https://<usuario>.github.io/<repo>/` y el agente en `.../agente/`.

## API key del agente
`agente/index.html` trae el marcador `__FLOW_API_KEY__` en lugar de una key real. **No subas una API key a GitHub**: queda pública y Anthropic la revoca automáticamente al detectarla. Para usar el agente, reemplaza el marcador solo en una copia local o en un hosting privado, con una key de un workspace con límite de gasto.

Autor: Camilo Melo
