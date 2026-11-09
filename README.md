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

- **Unidad 1, comandos:** 47 tarjetas con funciones tratadas en los PDF. Modos Elegir, Escribir, ¿Qué equipo?, Tarjetas, Protocolos, Terminal guiado y Biblioteca.
- **20 preguntas breves** sobre protocolos, puertos, servicios y diagnóstico de los PDF.
- **5 secuencias guiadas de TecnoRed:** interfaces de R1, administración del switch, SSH, seguridad básica y diagnóstico.
- **Unidad 2, subredes:** calculadora IPv4, asignación VLSM, ejercicios y direccionamiento del caso TecnoRed.
- **Sección Conceptos:** las 11 preguntas de análisis de la guía, con espacio para explicar, respuesta de referencia de la pauta, tres ideas clave, ejemplo y autoevaluación. Puedes marcar las que necesitas repasar.
- **Tres temas: Claro, Oscuro y AMOLED**, con la preferencia guardada. Oscuro conserva la paleta verde anterior; AMOLED utiliza negro puro (`#000000`) en el fondo, los paneles, los campos y la barra inferior, con texto blanco o gris claro y acentos suaves para distinguir acciones. La primera visita comienza en Oscuro.
- Progreso automático en el navegador, exportación e importación de estados JSON, restablecimiento y botones para deshacer y rehacer.

Las rondas tienen hasta 10 preguntas. Se priorizan las tarjetas con menor nivel y los errores pendientes. Una tarjeta se considera dominada después de 3 aciertos seguidos. Un error reinicia su nivel. En Tarjetas, la evaluación es personal. Mostrar la solución en el terminal cuenta como ayuda y ese paso no suma un acierto de memoria.

En Conceptos la respuesta escrita no se califica automáticamente: compárala con la pauta y marca si pudiste explicarla o necesitas repasarla. El borrador, la pregunta actual y esa evaluación se guardan con tu progreso.

En teléfonos se utilizan controles táctiles de al menos 44 píxeles en las acciones principales y campos de escritura de 16 píxeles para evitar el zoom automático de iOS. La barra inferior se oculta mientras escribes y vuelve al terminar.

## Guardar y recuperar avance

El progreso pertenece al navegador y al origen de la página. No se sincroniza entre dispositivos. El avance al abrir el archivo local y el avance de la página publicada se almacenan por separado.

- **Guardar:** descarga un archivo JSON con el progreso, filtros, ronda, posición en las secuencias, tema y respuestas conceptuales.
- **Cargar:** restaura un archivo de estado, también en otro dispositivo.
- **Restablecer:** comienza de cero, tras una confirmación.
- **↶ / ↷:** deshace o rehace hasta 40 cambios de la sesión actual. El historial de estos botones no se conserva al recargar ni se incluye en las copias.

Conserva copias JSON si quieres volver a distintos puntos de tu estudio. Si el navegador no permite almacenamiento local, la página lo indica y puedes usar Guardar estado. Cargar una copia reemplaza el estado actual; puedes deshacer la carga durante la misma sesión.

## Contenido y alcance

Fuentes proporcionadas:

- `Actividad Repaso - Certamen 2 - PAUTA DOCENTE.pdf`: solución de referencia TecnoRed.
- `Actividad Repaso - Certamen 2.pdf`: guía del estudiante.

El contenido académico se limita a esos dos PDF. Se retiraron las ampliaciones de comandos y el caso del documento Word. Las guías utilizan tres LAN conectadas directamente a un router 2911 y switches 2960, con VLAN 1 para administración. No se incluyen prácticas de VLAN adicionales, enlaces troncales ni rutas estáticas.

Las preguntas de Conceptos corresponden a las preguntas 1 a 11 del PDF del estudiante. Sus respuestas resumen la pauta docente y utilizan ejemplos del mismo caso. Las contraseñas, los textos y los nombres de archivos de los comandos son valores de práctica; las funciones son las tratadas en los PDF.

Las copias anteriores siguen siendo compatibles: se conserva el progreso de las tarjetas vigentes y se descartan las tarjetas o casos retirados. Si una ronda antigua contiene opciones de comandos retirados, se inicia una ronda actualizada.

El terminal guiado es una práctica de sintaxis por pasos. No es un emulador IOS y no verifica una topología real. Los comandos admitidos y los nombres de interfaz pueden variar por imagen y modelo de Packet Tracer. Se aceptan las abreviaciones y equivalencias documentadas en la biblioteca; no todas las abreviaciones posibles de IOS.

En los servidores de estas guías, DHCP, DNS, HTTP y FTP se configuran desde la pestaña **Services** de Packet Tracer. TCP y UDP son protocolos, no comandos. Las contraseñas incluidas son ejemplos de laboratorio.

Referencias adicionales:

- [Cisco: IP de administración y gateway del Catalyst 2960](https://www.cisco.com/c/en/us/td/docs/switches/lan/catalyst2960/software/release/15-0_2_se/configuration/guide/scg2960/swipaddr.html)
- [Cisco: configuración de SSH](https://www.cisco.com/c/en/us/support/docs/security-vpn/secure-shell-ssh/4145-ssh.html)

## Verificación realizada

Se probaron en Microsoft Edge las respuestas, los cinco recorridos guiados, los once ejercicios conceptuales, los borradores, la autoevaluación, el repaso, el guardado, la carga, el historial y la migración del progreso anterior. Las vistas se revisaron a 320, 375, 390, 430, 667, 768 y 1440 píxeles. El tema AMOLED se comprobó aparte en computador y móvil: negro puro en las superficies principales, contraste del texto, persistencia al recargar y carga de estados guardados.

También se probaron perfiles táctiles de iPhone 13 y Pixel 7 mediante emulación en Chromium. Esa emulación comprueba tamaños, interacción y comportamiento adaptable; no equivale a una prueba física en Safari de iOS o en un teléfono Android.

El diseño es adaptable y utiliza funciones web estándar de navegadores modernos. No se realizó una prueba física en Android o iPhone ni un despliegue en tu cuenta de Vercel.

## Modificar la página

Todo está en `index.html`: primero los estilos, luego los datos (`CARDS`, `CONCEPTS`, `SCENARIOS` y `THEORY`) y finalmente la lógica. Puedes editarlo y subir los cambios a GitHub para que Vercel los publique.

Proyecto de estudio independiente, sin afiliación con Cisco.
