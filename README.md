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

- **Selector de caso:** TecnoRed (PDF y pauta docente) o LogiSur (actividad en casa). La elección cambia las direcciones, equipos, dominios, requisitos, tarjetas, terminales y preguntas del resto de la página.
- **Unidad 1, comandos:** 47 tarjetas para TecnoRed y 49 para LogiSur. Modos Elegir, Escribir, ¿Qué equipo?, Tarjetas, Protocolos, Terminal guiado y Biblioteca. Cada ejercicio incluye “¿Dónde escribo este comando?”, con el recorrido hasta el equipo y modo correspondientes.
- **Preguntas breves de protocolos y diagnóstico:** 20 para TecnoRed y 22 para LogiSur.
- **5 secuencias guiadas por caso:** interfaces de R1, administración del primer switch, SSH, seguridad básica y diagnóstico.
- **Unidad 2, subredes:** calculadora IPv4, asignación VLSM, ejercicios y direccionamiento de ambos casos.
- **Sección Conceptos:** 11 preguntas de TecnoRed y 12 de LogiSur, con espacio para explicar, respuesta de referencia, ideas clave, ejemplo y autoevaluación. Las respuestas de LogiSur se elaboraron para estudiar: su DOCX no incluye pauta de soluciones.
- **Sección Laboratorio:** “Configurar la red” con cuatro encargos (router y switches, seguridad y SSH, servicios y PC, red completa) y “Completar bloques” con seis ejercicios por caso.
- **Tres temas: Claro, Oscuro y AMOLED**, con la preferencia guardada. Oscuro conserva la paleta verde anterior; AMOLED utiliza negro puro (`#000000`) en el fondo, los paneles, los campos y la barra inferior, con texto blanco o gris claro y acentos suaves para distinguir acciones. La primera visita comienza en Oscuro.
- Progreso automático en el navegador, exportación e importación de estados JSON, restablecimiento y botones para deshacer y rehacer.

Las rondas tienen hasta 10 preguntas. Se priorizan las tarjetas con menor nivel y los errores pendientes. Una tarjeta se considera dominada después de 3 aciertos seguidos. Un error reinicia su nivel. En Tarjetas, la evaluación es personal. Mostrar la solución en el terminal cuenta como ayuda y ese paso no suma un acierto de memoria.

En Conceptos la respuesta escrita no se califica automáticamente: compárala con la explicación de referencia y marca si pudiste explicarla o necesitas repasarla. El borrador y esa evaluación se guardan con tu progreso.

## Cómo usar Laboratorio

Elige TecnoRed o LogiSur en el selector existente y entra en **Laboratorio**. En **Configurar la red**, selecciona un encargo y un equipo. El esquema indica qué interfaz de R1 conecta cada LAN. La consola conserva el modo actual de cada dispositivo y muestra su prompt: `>`, `#`, `(config)#`, `(config-if)#` o `(config-line)#`.

Escribe los comandos en el orden que decidas. La práctica valida el contexto y actualiza el modelo: una IP se coloca dentro de una interfaz; el gateway del switch va en configuración global; `login local` y `transport input ssh` pertenecen a VTY. Si te equivocas de lugar, la consola explica cómo llegar al modo correcto.

- Usa **Tab** para completar un prefijo y **?** para consultar comandos del modo actual. En teléfono hay botones equivalentes.
- Usa ↑/↓ para recuperar comandos. No es necesario escribir el prompt.
- `show running-config`, `show ip interface brief` y `show ip route` muestran valores derivados de lo que configuraste.
- `copy running-config startup-config` pide confirmar el nombre de destino con Enter. Si luego modificas la configuración, el objetivo de guardado vuelve a quedar pendiente.
- Los objetivos indican qué falta y ofrecen una pista “¿Dónde va?”. La configuración y las sesiones son independientes por caso y encargo.
- En **Servicios y PC** se ensayan los campos de Services y Desktop de Packet Tracer: DHCP, DNS, HTTP, FTP y configuración de PC. Desde las PC se comprueban DHCP, ping, tracert, nslookup, FTP y SSH.
- **Completar bloques** ejercita partes faltantes de configuraciones con el prompt visible. La corrección explica el motivo de cada línea.

El laboratorio es un modelo didáctico de las funciones de estas guías, no una implementación completa de IOS ni un simulador de paquetes. El cableado se da por conectado. El acceso SSH y las pruebas de servicios dependen de la configuración de este modelo; comprueba después la configuración real en Packet Tracer. Las claves utilizadas aquí deben ser credenciales de práctica.

En teléfonos se utilizan controles táctiles de al menos 44 píxeles en las acciones principales y campos de escritura de 16 píxeles para evitar el zoom automático de iOS. La barra inferior se oculta mientras escribes y vuelve al terminar.

## Guardar y recuperar avance

El progreso pertenece al navegador y al origen de la página. No se sincroniza entre dispositivos. El avance al abrir el archivo local y el avance de la página publicada se almacenan por separado.

- **Guardar:** descarga un archivo JSON con el progreso, caso, filtros, ronda, posición en las secuencias, tema, respuestas conceptuales y configuraciones del laboratorio.
- **Cargar:** restaura un archivo de estado, también en otro dispositivo.
- **Restablecer:** comienza de cero, tras una confirmación.
- **↶ / ↷:** deshace o rehace hasta 40 cambios de la sesión actual. El historial de estos botones no se conserva al recargar ni se incluye en las copias.

Conserva copias JSON si quieres volver a distintos puntos de tu estudio. Si el navegador no permite almacenamiento local, la página lo indica y puedes usar Guardar estado. Cargar una copia reemplaza el estado actual; puedes deshacer la carga durante la misma sesión.

## Contenido y alcance

Fuentes proporcionadas:

- `Actividad Repaso - Certamen 2 - PAUTA DOCENTE.pdf`: solución de referencia TecnoRed.
- `Actividad Repaso - Certamen 2.pdf`: guía del estudiante.
- `Actividad_Repaso_Certamen2_Casa.docx`: actividad LogiSur, reincorporada a petición del usuario.

El contenido académico sigue las funciones tratadas en esas guías. Ambas usan tres LAN conectadas directamente a un router 2911 y switches 2960, con VLAN 1 para administración. No se incluyen prácticas de VLAN adicionales, enlaces troncales ni rutas estáticas. LogiSur añade el ejercicio de deshabilitar/restaurar una interfaz, una falla de máscara, DHCP DORA y carga FTP cuando esté disponible.

Las preguntas de Conceptos corresponden a las preguntas 1 a 11 del PDF y 1 a 12 del DOCX. TecnoRed resume la pauta docente. Las explicaciones de LogiSur se elaboraron a partir de los conceptos de su actividad y se identifican como tales. Las contraseñas, textos y nombres de archivo son valores de práctica.

Las copias anteriores siguen siendo compatibles. Las nuevas tarjetas de LogiSur guardan su progreso por separado del de TecnoRed. Si una ronda antigua contiene opciones que ya no pertenecen a su caso, se inicia una ronda actualizada.

El terminal guiado es una práctica de sintaxis por pasos. No es un emulador IOS y no verifica una topología real. Los comandos admitidos y los nombres de interfaz pueden variar por imagen y modelo de Packet Tracer. Se aceptan las abreviaciones y equivalencias documentadas en la biblioteca; no todas las abreviaciones posibles de IOS.

En los servidores de estas guías, DHCP, DNS, HTTP y FTP se configuran desde la pestaña **Services** de Packet Tracer. TCP y UDP son protocolos, no comandos. Las contraseñas incluidas son ejemplos de laboratorio.

Referencias adicionales:

- [Cisco: IP de administración y gateway del Catalyst 2960](https://www.cisco.com/c/en/us/td/docs/switches/lan/catalyst2960/software/release/15-0_2_se/configuration/guide/scg2960/swipaddr.html)
- [Cisco: configuración de SSH](https://www.cisco.com/c/en/us/support/docs/security-vpn/secure-shell-ssh/4145-ssh.html)

## Verificación realizada

Se probaron en Microsoft Edge las funciones anteriores y las nuevas prácticas: cuatro encargos y seis bloques en los dos casos, rechazo de comandos en modo incorrecto, configuración de red, SSH con autenticación, DHCP, DNS, HTTP, FTP, guardado/restauración, historial y cambio de caso en las distintas secciones. También se verificó que apagar/restaurar G0/2 en LogiSur cambie el resultado de las pruebas y que un cambio posterior al guardado deje la configuración pendiente de guardar.

El laboratorio se revisó en Claro, Oscuro y AMOLED a 320, 390, 768 y 1440 píxeles. Las revisiones anteriores cubrieron además 375, 430 y 667 píxeles. Los menús desplegables tienen colores explícitos para mantener legibles las opciones en AMOLED.

También se probaron perfiles táctiles de iPhone 13 y Pixel 7 mediante emulación en Chromium. Esa emulación comprueba tamaños, interacción y comportamiento adaptable; no equivale a una prueba física en Safari de iOS o en un teléfono Android.

El diseño es adaptable y utiliza funciones web estándar de navegadores modernos. No se realizó una prueba física en Android o iPhone ni un despliegue en tu cuenta de Vercel.

## Modificar la página

Todo está en `index.html`: primero los estilos, luego los datos de ambos casos y el modelo del laboratorio, y finalmente la lógica y las vistas. Puedes editarlo y subir los cambios a GitHub para que Vercel los publique.

Proyecto de estudio independiente, sin afiliación con Cisco.
