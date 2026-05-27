> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://github.com/mintlify/docs --skill mintlify`

# Centro de ayuda de Asentado — instrucciones del proyecto

## Sobre este proyecto

- Es el centro de ayuda de **Asentado**, la plataforma de gestión de Higiene y Seguridad para consultoras.
- Sitio de documentación construido sobre [Mintlify](https://mintlify.com).
- Las páginas son archivos MDX con frontmatter YAML. La configuración vive en `docs.json`.
- Corré `mint dev` para previsualizar localmente y `mint broken-links` para chequear enlaces.

## Alcance del help

- **Solo** usuarios de la consultora: el admin (panel web) y el prevencionista (app móvil).
- El sitio está en **español rioplatense**. Se permite y se prefiere el voseo.

## Terminología

Usá siempre estos términos. La columna "No usar" lista alternativas a evitar.

| Término | No usar |
|---|---|
| Consultora | partner, organización |
| Cliente | empresa vinculada |
| Obra | espacio, sitio, proyecto |
| Prevencionista | técnico, preventista |
| Visita | fichaje |
| Formulario | plantilla, constancia template |
| Reporte de formulario | constancia |
| Hallazgo | observación, no conformidad |
| Cuasi accidente | casi accidente, near miss |
| Ticket | tarea, pendiente |
| Ticketera | — |
| Documentación | documentos, carpeta |
| Vencimientos | alertas |
| Recurso | — |
| Planificación | gantt |

## Preferencias de estilo

- Tono cercano y directo. Verbos en imperativo voseante: "Tocá", "Hacé clic", "Ingresá".
- Voz activa y segunda persona ("vos").
- Frases concisas: una idea por oración.
- Una acción por paso. Usá el componente `<Steps>` para los procedimientos numerados.
- Títulos en sentence case (mayúscula solo en la primera palabra).
- Negrita para elementos de UI: hacé clic en **Configuración**.
- Formato de código para nombres de archivo, comandos, rutas, valores literales (`1234`, `DD/MM/AAAA`, `tecnico`) y rutas de la app (`/partner/empresa/<slug>`).
- Nunca uses jerga interna: no menciones "RLS", "shadow", "policies", "migraciones" ni "Supabase".

## Límites de contenido

No documentar:

- Flujos del **admin de la empresa cliente** (tienen su propio help aparte).
- Setup técnico (Supabase, RLS, migraciones, triggers).
- Configuración super-admin de Asentado.
- Edge cases técnicos (rate limits, etc.).
- Las features premium gateadas solo se mencionan al pasar ("si tu cliente tiene contratado el módulo X"), nunca se documentan en detalle.
