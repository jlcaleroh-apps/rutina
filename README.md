# Mi Rutina

Temporizador visual (tipo Time Timer de 60 min) con rutina de actividades, checklist y rachas. Pensado para iPad, en español e inglés.

- Archivo: `index.html` (una sola página, sin instalación).
- Para usarla: abre la página en Safari y toca **Compartir → Agregar a pantalla de inicio** (tiene ícono propio y se abre a pantalla completa). En Android/Chrome: menú ⋮ → Instalar app.
- Los perfiles, rutinas y el progreso se guardan solo en el navegador de cada dispositivo.
- Funciona sin internet después de abrirla una vez con conexión (`sw.js`). Si cambias íconos o agregas archivos, sube la versión de `CACHE` en `sw.js`.
- Sin PIN por defecto: cualquiera puede abrir ⚙️ Ajustes. Se puede poner un PIN opcional en ⚙️ Ajustes → General.
- La primera vez, una bienvenida de 3 pasos pide el nombre del niño o la niña y la rutina inicial.
- Botón ❓: explica los principios para TDAH en que se basa la app y cómo usarla (se muestra sola la primera vez).

## Componentes comunes (iguales en todas las apps de jlcaleroh-apps)
Esta app sigue el [estándar común](https://github.com/jlcaleroh-apps/plantilla/blob/main/ESTANDAR.md). Las apps nuevas se crean desde [plantilla](https://github.com/jlcaleroh-apps/plantilla).

- **`respaldo.js` · Respaldo del progreso:** en el panel del adulto, "Guardar respaldo" crea un archivo con el progreso de todos los niños (se guarda en Archivos, AirDrop o correo) y "Restaurar respaldo" lo carga en este u otro iPad. Muestra la fecha del último respaldo y avisa si pasaron más de 2 semanas. También pide al iPad que no borre los datos de la app.
  - Es el mismo archivo en todas las apps: si se mejora, se copia igual en cada repo.
  - Cada app declara qué claves de almacenamiento son suyas, porque todas comparten el dominio `jlcaleroh-apps.github.io`.

## Contacto
jlcaleroh@gmail.com
