# VIDRATEMP

Demostración de un sistema de gestión para **Vitrotemp Ltda.**, empresa de importación,
corte y templado de vidrio en La Paz. Tres aplicaciones, cada una un único archivo HTML
que se abre con doble clic, sin servidor ni compilación.

| Aplicación | Archivo | Para quién |
|---|---|---|
| **Portal de demostración** | [`index.html`](index.html) | Describe las tres pantallas y abre cada una |
| **VIDRATEMP Web** | [`vidratemp-web.html`](vidratemp-web.html) | Oficina: dirección, ventas, producción, almacén y administración |
| **VIDRATEMP Móvil** | [`vidratemp-movil.html`](vidratemp-movil.html) | Planta y almacén: recepción, lectura de códigos, retazos, avance de producción |
| **Seguimiento de pedido** | [`vidratemp-seguimiento.html`](vidratemp-seguimiento.html) | Cliente final: enlace personal con el avance de su pedido |

## VIDRATEMP Web

Sistema completo con 17 vistas en cuatro grupos (Operación, Planta, Existencias, Gestión)
y acceso por rol. Incluye tres motores de cálculo:

- **Precios** — cotización por m² con mínimo facturable, procesos por ml / m² / unidad y
  recargo por urgencia; valida cada pieza contra la chapa, el espesor templable y la cama del horno.
- **Agenda de capacidad** — promete fecha de entrega según la carga real de los próximos
  ocho días (temple, corte y entregas por día).
- **Optimizador de corte** — empaqueta las piezas en la chapa (MaxRects con rotación, kerf y
  refile), dibuja el plano, registra los sobrantes como retazos y exporta DXF para la cortadora.

Usuarios de demostración: cinco roles, contraseña `demo1234`.

## VIDRATEMP Móvil

Aplicación del piso de planta, en cinco pestañas: Inicio, Leer (lector de códigos con
acciones de contexto), Recepción (conferencia de contenedor contra factura), Retazos
(búsqueda de sobrantes por medida y alta con etiqueta) y Planta (avance por etapa,
despachos y estado del horno). Los retazos registrados se guardan en el navegador.

## Seguimiento de pedido

Página que recibe el cliente por WhatsApp: etapa actual, avance con hora de cada sello,
fecha de entrega comprometida, detalle de piezas y resumen de pago. Tres pedidos de
ejemplo para alternar.

## Notas

- Un solo lenguaje visual en las tres pantallas (fuentes Archivo y Archivo Narrow, cargadas
  de Google Fonts); tema claro y oscuro según el sistema.
- Fechas, horas y montos en formato `es-BO`; moneda en bolivianos.
- Los datos (clientes, pedidos, importaciones, personal) son ficticios y coherentes entre sí.

---

Emergeware Technologies · 2026
