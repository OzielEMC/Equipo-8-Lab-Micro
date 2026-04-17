Altavoz de Radio por Internet con ESP32

Descripción del proyecto

El presente proyecto consiste en el desarrollo de un dispositivo basado en el microcontrolador ESP32 capaz de reproducir estaciones de radio por internet en tiempo real. Este sistema utiliza una conexión WiFi para acceder a un flujo de audio en formato MP3, el cual es procesado y convertido en sonido audible mediante un módulo DAC y una bocina.

Permite reproducir audio en línea sin necesidad de computadora o teléfono
Demuestra el uso de streaming en sistemas embebidos
Integra comunicación inalámbrica, procesamiento y salida de audio

Arquitectura del sistema

El funcionamiento del sistema se divide en varias etapas que trabajan de manera continua:

Entrada: Se obtiene el flujo de audio desde una URL de radio en línea
Comunicación: El ESP32 se conecta a la red WiFi y recibe los datos
Procesamiento: Se decodifica el audio MP3 mediante una librería
Salida: El DAC convierte la señal digital en analógica y la bocina reproduce el sonido

Diagrama de flujo

El comportamiento del sistema sigue una secuencia lógica:

Inicialización del sistema
Conexión a la red WiFi
Verificación de conexión
Configuración de pines I2S
Conexión al servidor de radio
Recepción y decodificación del audio
Envío de señal al DAC
Reproducción en la bocina
Repetición continua del proceso

Tecnologías utilizadas

Para la implementación del proyecto se utilizaron los siguientes elementos:

Hardware:
ESP32
Módulo DAC MAX98357A
Bocina de 8Ω y 3W
Software:
Arduino IDE
Librería WiFi.h
Librería Audio.h
Monitor serial para depuración

Estructura del proyecto

El proyecto está organizado de forma sencilla:

Archivo principal con la lógica del sistema
Carpeta de documentación (diagramas y explicaciones)
Carpeta de recursos (imágenes o evidencias)
Archivo README con la descripción general

Requisitos e instalación

Para ejecutar el proyecto se necesita:

ESP32
Módulo DAC
Bocina
Arduino IDE instalado

Pasos generales:

Instalar Arduino IDE
Configurar soporte para ESP32
Instalar la librería de audio
Conectar el hardware correctamente

Cómo usarlo

El uso del sistema es directo y no requiere interacción constante:

Abrir el código en Arduino IDE
Configurar red WiFi (nombre y contraseña)
Configurar la URL de la radio
Cargar el programa al ESP32
El sistema se ejecuta automáticamente

Cómo correr pruebas

La validación se realiza mediante pruebas simples:

Verificar conexión WiFi
Confirmar conexión con el servidor
Escuchar audio en la bocina
Revisar mensajes en el monitor serial

FAQ — Dudas frecuentes

No se escucha audio:
Revisar conexiones del DAC y bocina, además de la URL
No conecta a WiFi:
Verificar credenciales
¿Se puede cambiar la estación?
Sí, modificando la URL en el código
¿Necesita servidor?
No, todo funciona directamente en el ESP32

Cómo contribuir

Si alguien desea mejorar el proyecto puede:

Clonar el repositorio
Crear una nueva versión o mejora
Agregar funcionalidades (más estaciones, interfaz, etc.)
Documentar los cambios realizados

Resumen general

Este proyecto demuestra cómo es posible construir un sistema funcional de audio por internet utilizando un microcontrolador, integrando conceptos de programación, electrónica y redes. Además, permite comprender de manera práctica cómo fluye la información desde internet hasta convertirse en sonido, reforzando el aprendizaje de forma clara y aplicada.
