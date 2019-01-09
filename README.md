# fona_foun
Creando un teléfono a partir del Fona de Adafruit

## Intro

Nunca me han gustado los teléfonos "inteligentes", y me parece que son la peor computadora de todas las que he utilizado. Mi teléfono de marca no rinde la batería, y volvió a inflar otr LiPo, por lo cual decidí pasarme a una plataforma donde uno tenga el control sobre lo que sucede en el software, así como usar APIs públicos para crear reemplazos de las pocas aplicaciones que uso de vez en cuando.


## TODO:
- [√] Batería 18650
- [x] Pantalla Feather OLED: No se puede con At32u4
- [ ] Placa administradora por serial
- [ ] FONAtest en pantalla OLED
- [ ] Ring en parlante
- [ ] Medir batería
- [ ] Aceptar llamada
- [ ] Rechazar llamada
- [ ] Mute Ring
- [ ] Vibrador
- [ ] Marcar número
- [ ] Agenda
- [ ] Redial
- [ ] Menu
- [ ] Recibir SMS
- [ ] Enviar SMS
- [ ] Notificación SMS
- [ ] Teclado
- [ ] GPS
- [ ] Uber
- [ ] Telegram
- [ ] Tether de 3G a wifi

## Problemas:
- Micros pequeñas: La Atmel 32u4 que tiene la Fona, tiene funcionalidades interesantes como HID USB, sin embargo no tiene suficiente capacidad para manejar tanto la librería de Fona, como la librería de OLED, por lo cual es necesario utilizar una micro con más poder, como una m0, m4 o STM32, la cual controla tanto el Fona como la pantalla, por medio de comandos seriales.
