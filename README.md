# USM PRF — Registro del proyecto

Ubicación: C:\Users\OmarAdrian\Documents\development\workspace\Morna\usm\prf
Inicio: 2025-10-31

Este archivo centraliza cambios, bugs críticos y tareas por hacer del proyecto.

## Registro de Cambios

Sigue el formato: Added, Changed, Fixed, Removed, Security.

### [Unreleased] - 2025-10-31
- Added:
  - Archivo app.js con la lógica de la aplicación.
  - Archivo styles.css con estilos y reglas de impresión.
- Changed:
  - index.html ahora enlaza assets externos y elimina CSS/JS embebido.
- Fixed:
- Removed:
- Security:

## Bugs críticos

Plantilla para cada bug crítico:
- ID: BUG-YYYY-001
  - Fecha: 2025-10-31
  - Estado: Abierto | Mitigado | Resuelto
  - Descripción: 
  - Impacto: 
  - Reproducción: 
  - Propietario: 
  - Notas: 

## Tareas por hacer

Prioriza con P1 (alto), P2 (medio), P3 (bajo).
- P1
  - [ ] 
- P2
  - [ ] 
- P3
  - [ ] 

## Flujo recomendado
- Crea rama por feature/bugfix.
- Documenta cambios en "Unreleased" al commitear.
- Mueve items a versión cuando se libere (e.g., 0.1.0 - YYYY-MM-DD).
- Registra bugs críticos con la plantilla y vínculo al issue.

## Configuración: Supabase (Autenticación)

Para usar la autenticación con Supabase (registro/login de usuarios) en este proyecto:

- Crea un proyecto en https://supabase.com y copia tu Project URL y anon/public API key.
- En `index.html` se incluye un ejemplo que inicializa el cliente Supabase vía CDN. Puedes reemplazar las constantes por tus valores o preferir usar bundler y variables de entorno.
- No expongas la service_role key en cliente. Úsala solo en servicios backend.

Prueba rápida local (sin bundler): abre `index.html` en un navegador; el script ya cargará el cliente desde CDN. En la pantalla de inicio verás formularios para registro y login de usuario (lado derecho). Para pruebas completas con un bundler, instala `@supabase/supabase-js`:

```powershell
npm install @supabase/supabase-js
```


## Convención de commits (sugerida)
feat:, fix:, docs:, refactor:, perf:, test:, build:, ci:, chore:, style:, revert:
