# Juanlu Rodríguez · Fisioterapia

Landing Astro para pacientes de fisioterapia en Inca y online. Terapia manual, ejercicio terapéutico, punción seca y electropunción. Primera sesión presencial 60 €, seguimiento 55 €, consulta online 40 €.

## Desarrollo

Node 22. Ejecutar `npm ci`, `npm run dev` y `npm run build`. La salida estática se genera en `dist` y puede alojarse en Cloudflare Pages sin adaptadores.

La web permite solicitar cita por correo; abrir el mensaje no lo envía ni confirma la cita. El setter y la agenda no están conectados. La imagen utiliza la URL pública de la web personal existente.

`PUBLIC_PATIENT_BOOKING_URL` permite añadir una agenda verificada de pacientes de forma opcional. Véase `.env.example`. Si no se configura, se muestra únicamente la solicitud por correo.

No se incluyen cookies analíticas, almacenamiento de datos de pacientes ni formularios clínicos en esta landing.
