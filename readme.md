# QuakeTimer

## Descripción

**QuakeTimer** es un temporizador visual de dos colores (verde y rojo) pensado para juegos o actividades rápidas, con control por voz y visualización de audio en tiempo real.  
Permite iniciar, pausar y reiniciar los temporizadores tanto por clic como por comandos de voz ("escudo", "mega", "pausa", "sigue").  
Incluye una barra de visualización de audio y es compatible con escritorio y dispositivos móviles en red local.

---

## Características

- Dos temporizadores independientes: **ESCUDO** (verde) y **MEGA** (rojo).
- Control por voz (palabras clave: "escudo", "mega", "pausa", "sigue").
- Visualización de la actividad del micrófono en la parte superior.
- Botón central **GO!** para activar el reconocimiento de voz y el visualizador.
- Compatible con navegadores modernos (Chrome recomendado).
- Funciona en red local (acceso desde otros dispositivos usando la IP local).

---

## Uso en red local (PC y móvil)

1. Asegurarse tener PC y tu telefono en la misma red WiFi.
2. Ejecuta un servidor local en la carpeta del proyecto. Ejemplo con Python:
   ```
   python -m http.server 8000
   ```
3. Desde tu celu, abrir el browser y acceder a:
   ```
   http://[IP-de-tu-PC]:8000/
   ```
   (Reemplazar `[IP-de-tu-PC]` por la IP local de tu compu).

---

## Requisitos

- Navegador moderno con soporte para reconocimiento de voz y acceso a micrófono.
- Permitir acceso al micrófono cuando lo solicite el navegador.

---

## Comandos de voz soportados

- **"escudo"**: reinicia el temporizador verde.
- **"mega"**: reinicia el temporizador rojo.
- **"pausa"**: pausa el temporizador activo.
- **"sigue"**: reanuda el temporizador pausado.

---

## Notas

- En algunos tel, el reconocimiento de voz y el acceso al micrófono pueden requerir HTTPS.
- Si tenes problemas de permisos, revisa la configuración de tu navegador.
- El temporizador baja de 30 a 29 a los 500 ms para mayor agilidad visual.

---

## Créditos

Desarrollado por CristianSan