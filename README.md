# sistema-besabik-demo

Demo navegable del **sistema de gestión** de Centro Estético Besabik (Gualaceo, Azuay · Ecuador).

Es el complemento de la landing: la web pública atrae y agenda; este panel es lo que el centro usa todos los días.

## Qué incluye

Aplicación de una sola página (`index.html`, CSS y JS inline, sin backend ni dependencias externas salvo Google Fonts):

- **Entrada simulada**: usuario demo precargado y botón «Entrar en modo demostración» (sin autenticación real).
- **Escritorio**: citas de hoy, ocupación, ingresos del día, próximas citas, avisos (mensajes por responder, recordatorios por enviar, packs por vencer, cobros pendientes) y últimos cobros.
- **Agenda**: vista de semana y de día por profesional, con detalle de cada cita y creación real de citas desde el formulario (clienta, servicio, profesional, día, hora, duración). Avisa si se cruza el horario de una profesional.
- **Clientas**: buscador, listado y ficha con contacto, historial de visitas, packs con sesiones usadas y restantes, notas y fotos de evolución (simuladas).
- **Mensajes**: bandeja tipo WhatsApp con recordatorios automáticos, confirmaciones y reprogramaciones; se ve el flujo «recordatorio 24 h antes → confirmación».
- **Pagos**: cobros del mes con fecha, clienta, servicio, método (efectivo, transferencia, tarjeta) y estado (pagado / pendiente), con totales y ticket promedio.
- **Informes**: citas por semana, estado de las citas (donut), servicios más vendidos, ingresos por mes y ocupación por profesional. Todo hecho con SVG y CSS, sin librerías.
- **Ajustes**: catálogo de servicios editable en memoria (precio y duración), horarios de atención y configuración del recordatorio automático (cuántas horas antes), con vista previa del mensaje.
- Menú de usuario con acceso a la web pública del centro, y pie con la nota de demo.

Los datos son de ejemplo y se generan en el navegador, relativos a la fecha en que se abre el demo: 30 clientas, unas 90 citas repartidas en el mes, 8 packs, pagos en dólares y tres profesionales (Karla, Doménica y Andrea).

## Despliegue

`Dockerfile` de dos líneas (`nginx:alpine` + copia de los archivos) publicado desde este repositorio en EasyPanel:

- Sistema: https://clientes-sistema-besabik.rddxeh.easypanel.host/

## Nota

Demo de referencia hecho por Nocodeveloper. No envía mensajes, no guarda datos y no incluye información real de terceros; en el sistema real se cargan los datos del centro.
