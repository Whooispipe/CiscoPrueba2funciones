# Cisco práctica para el certamen 2

Página de estudio en español, adaptable a computadores, tablets y teléfonos. HTML, CSS y JavaScript en un solo `index.html`, sin dependencias, cuentas ni base de datos.

## Abrir ahora

Abre `index.html` en un navegador moderno. Para usarla desde Android o iPhone, publica el repositorio en Vercel y abre su enlace en el navegador del dispositivo.

## Publicar con GitHub y Vercel

1. Sube **el contenido de esta carpeta** a tu repositorio GitHub. `index.html`, `vercel.json` y este archivo deben estar en la raíz del repositorio, no dentro de otra carpeta adicional.
2. En Vercel, elige **Add New → Project** e importa el repositorio.
3. Usa **Framework Preset: Other** y la raíz del repositorio como **Root Directory**.
4. El archivo `vercel.json` ya configura una página estática: no hay comando de instalación ni compilación. La carpeta de salida es `.`.
5. Pulsa **Deploy** y abre el enlace que genere Vercel. Ese mismo enlace sirve para Windows, Android e iOS.

No se necesitan variables de entorno ni claves. Si Vercel solicita un comando de compilación, activa su opción de personalización y deja el campo vacío.

Referencia: [configuración oficial de proyectos estáticos en Vercel](https://vercel.com/docs/builds/configure-a-build#skip-build-step).

## Qué incluye

- **Unidad 1, comandos:** 63 tarjetas, incluidas 51 de la materia central y 12 extras de VLAN y diagnóstico. Modos Elegir, Escribir, ¿Qué equipo?, Tarjetas, Protocolos, Terminal guiado y Biblioteca.
- **22 preguntas** sobre protocolos, puertos, servicios y diagnóstico.
- **5 secuencias guiadas por caso:** interfaces de R1, administración del switch, SSH, seguridad básica y diagnóstico. Están disponibles tanto para TecnoRed como para LogiSur.
- **Unidad 2, subredes:** calculadora IPv4, asignación VLSM, ejercicios y tablas de direccionamiento de ambos casos.
- Progreso automático en el navegador, exportación e importación de estados JSON, restablecimiento y botones para deshacer y rehacer.

Las rondas tienen hasta 10 preguntas. Se priorizan las tarjetas con menor nivel y los errores pendientes. Una tarjeta se considera dominada después de 3 aciertos seguidos. Un error reinicia su nivel. En Tarjetas, la evaluación es personal. Mostrar la solución en el terminal cuenta como ayuda y ese paso no suma un acierto de memoria.

## Guardar y recuperar avance

El progreso pertenece al navegador y al origen de la página. No se sincroniza entre dispositivos. El avance al abrir el archivo local y el avance de la página publicada se almacenan por separado.

- **Guardar estado:** descarga un archivo JSON con el progreso, filtros, ronda y posición en las secuencias.
- **Cargar:** restaura un archivo de estado, también en otro dispositivo.
- **Restablecer:** comienza de cero, tras una confirmación.
- **↶ / ↷:** deshace o rehace hasta 40 cambios de la sesión actual. El historial de estos botones no se conserva al recargar ni se incluye en las copias.

Conserva copias JSON si quieres volver a distintos puntos de tu estudio. Si el navegador no permite almacenamiento local, la página lo indica y puedes usar Guardar estado. Cargar una copia reemplaza el estado actual; puedes deshacer la carga durante la misma sesión.

## Contenido y alcance

Fuentes proporcionadas:

- `Actividad Repaso - Certamen 2 - PAUTA DOCENTE.pdf`: solución de referencia TecnoRed.
- `Actividad Repaso - Certamen 2.pdf`: guía del estudiante.
- `Actividad_Repaso_Certamen2_Casa.docx`: caso LogiSur, sin soluciones. Sus tablas se calcularon a partir de los requisitos.

Las guías utilizan tres LAN conectadas directamente a un router 2911 y switches 2960. Solo requieren VLAN 1 para administración; las VLAN adicionales y los troncales están identificados como extras. No se agregan rutas estáticas a estos casos.

El terminal guiado es una práctica de sintaxis por pasos. No es un emulador IOS y no verifica una topología real. Los comandos admitidos y los nombres de interfaz pueden variar por imagen y modelo de Packet Tracer. Se aceptan las abreviaciones y equivalencias documentadas en la biblioteca; no todas las abreviaciones posibles de IOS.

En los servidores de estas guías, DHCP, DNS, HTTP y FTP se configuran desde la pestaña **Services** de Packet Tracer. TCP y UDP son protocolos, no comandos. Las contraseñas incluidas son ejemplos de laboratorio.

Referencias adicionales:

- [Cisco: IP de administración y gateway del Catalyst 2960](https://www.cisco.com/c/en/us/td/docs/switches/lan/catalyst2960/software/release/15-0_2_se/configuration/guide/scg2960/swipaddr.html)
- [Cisco: configuración de SSH](https://www.cisco.com/c/en/us/support/docs/security-vpn/secure-shell-ssh/4145-ssh.html)

## Verificación realizada

Se probaron en Microsoft Edge las respuestas, las equivalencias de comandos, los diez recorridos guiados (cinco por caso), el guardado y la carga, los archivos inválidos, el historial y el cálculo de subredes, incluidos /0, /31 y /32. Se revisó que las vistas no desborden horizontalmente a 320, 390, 768 y 1440 píxeles de ancho.

El diseño es adaptable y utiliza funciones web estándar de navegadores modernos. No se realizó una prueba física en Android o iPhone ni un despliegue en tu cuenta de Vercel.

## Modificar la página

Todo está en `index.html`: primero los estilos, luego los datos de las tarjetas (`CARDS`, `CONCEPTS`, `SCENARIOS`) y finalmente la lógica. Puedes editarlo y subir los cambios a GitHub para que Vercel los publique.

Proyecto de estudio independiente, sin afiliación con Cisco.
