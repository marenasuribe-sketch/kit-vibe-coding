# CLAUDE.md — Reglas del proyecto

> Copia este archivo a la raíz de tu proyecto. Claude Code lo lee automáticamente al iniciar cada sesión.
> Completa la sección "Sobre este proyecto" (o pídele a Claude: "lee el PRD en docs/PRD.md y completa la sección Sobre este proyecto del CLAUDE.md").
> Mantenlo corto: todo lo que escribas aquí se carga en cada sesión y gasta contexto.

## Sobre este proyecto
- **Qué es:** (una frase: qué hace la app y para quién)
- **Documento de producto:** `docs/PRD.md` — léelo antes de proponer funcionalidades nuevas.
- **Tecnología:** (ej. Next.js + Supabase + Tailwind, publicado en Vercel)
- **Idioma de la interfaz:** español neutro, tratando al usuario de "tú".
- **Moneda y país principal:** (ej. México, MXN · España, EUR · clientes internacionales, USD)

## Cómo trabajo con la dueña/el dueño del proyecto
- No soy programador. Explícame en español simple, sin jerga; si usas un término técnico, explícalo en una línea.
- Antes de cambiar más de 2 archivos o instalar algo, muéstrame un plan corto (qué archivos, qué cambia y por qué) y espera mi "ok".
- Si mi pedido es ambiguo, hazme como máximo 3 preguntas concretas antes de empezar.
- Al terminar cada tarea, dime: (1) qué cambiaste, (2) cómo lo pruebo yo, paso a paso, (3) qué quedó pendiente.

## Reglas de cambios
- Haz el cambio más pequeño que resuelva lo pedido. No refactorices, no renombres ni "mejores" código que no te pedí.
- Edita archivos existentes en vez de reescribirlos completos.
- Nunca borres archivos, tablas, columnas o datos sin preguntarme primero.
- No cambies la tecnología, las librerías principales ni la estructura de carpetas sin aprobación.
- No agregues dependencias nuevas si se puede resolver con lo que ya está instalado. Si necesitas una, dime cuál y por qué.
- Si algo no funciona después de 2 intentos, detente, explícame qué crees que pasa y propón 2 alternativas.

## Seguridad (no negociable)
- Jamás escribas claves, tokens o contraseñas en el código. Usa variables de entorno (`.env.local`) y verifica que `.env*` esté en `.gitignore`.
- Las claves secretas (clave secreta de Stripe, Client Secret de PayPal, Access Token de Mercado Pago, secretKey de Flow, service_role de Supabase, etc.) solo se usan en el servidor, nunca en código que corre en el navegador.
- Toda tabla con datos de usuarios debe tener reglas de acceso (RLS en Supabase / Security Rules en Firebase).
- Valida en el servidor todo lo que venga de formularios. Nunca confíes en precios o montos enviados desde el navegador.

## Calidad mínima
- Después de cada cambio, verifica que el proyecto compila/arranca (`npm run build` o el comando equivalente) y corrige los errores que causaste.
- Textos visibles en español, con tildes y signos de apertura (¿ ¡).
- Diseño responsive: debe verse bien en celular primero.
- Mensajes de error amables para el usuario final; los detalles técnicos van a la consola, no a la pantalla.

## Memoria entre sesiones
- Al terminar una sesión, actualiza `PROXIMA-SESION.md` (qué se hizo, qué falta, problemas abiertos) y agrega una línea en `CHANGELOG.md`.
- Al empezar, lee `PROXIMA-SESION.md` si existe.

## Comandos del proyecto
- Instalar: `npm install`
- Desarrollo: `npm run dev`
- Compilar: `npm run build`
(ajusta si tu proyecto usa otros comandos)
