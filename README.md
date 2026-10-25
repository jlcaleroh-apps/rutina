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
- **`voz.js` · Prueba de voz:** en el panel del adulto, elegir la voz del iPad para cada idioma, ajustar la velocidad y escuchar ejemplos de la app. Donde aplica, permite grabar tu propia voz para letras, sílabas o palabras sueltas; las grabaciones viajan en el respaldo.
- **`adulto.js` · Gesto del panel del adulto:** mantener presionado 2 segundos; el botón se llena de color y, si se suelta antes, aparece un aviso. Así los niños no lo abren por accidente.
- **`pantalla.js` · Pantalla encendida:** mientras el niño toca la pantalla, el iPad no se apaga; tras 3 minutos sin actividad se suelta para cuidar la batería.
- **`apps.js` · Otras apps:** en la ventana de información, enlaces a las demás apps de la colección (Robot Sílabo, Trazos de Arquitecto, Números, Mi Rutina) para que los padres conozcan las otras. Al crear una app nueva se agrega a su lista y se copia igual en todos los repos.

## Contacto
jlcaleroh@gmail.com
