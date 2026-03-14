Scripts desarrollados durante la materia de Ciberseguridad. El proyecto principal es una herramienta de análisis forense que permite revisar eventos críticos del sistema, conexiones de red activas y verificar la reputación de IPs externas.

El módulo principal tiene cuatro funciones. Una revisa el historial de eventos de Windows buscando cosas como inicios de sesión fallidos, procesos nuevos o servicios instalados recientemente. Otra analiza las conexiones TCP activas y te dice qué proceso las está usando y si el ejecutable está firmado digitalmente o no. También hay una función que consulta la API de AbuseIPDB para saber si una IP tiene reportes de actividad maliciosa. Por último hay una función que junta todo eso y genera un reporte en HTML.

El archivo Menu.ps1 es el que se ejecuta directamente y te da un menú para elegir qué quieres hacer.

Sirve para hacer una revisión rápida de un equipo cuando sospechas que algo raro está pasando. Puedes ver qué conexiones salientes tiene el equipo, si algún proceso desconocido está comunicándose hacia afuera, y si esas IPs ya han sido reportadas por otras personas como maliciosas.

Aprendimos a trabajar con módulos de PowerShell usando manifiesto .psd1, a consumir APIs externas con Invoke-RestMethod, a leer el registro de eventos de Windows con Get-WinEvent y a generar reportes HTML desde la terminal.

Equipo:
Eduardo Velazquez Zepeda
Fernando de Jesus Gutierrez Lopez
Pablo Javier Mora Delgadillo
Gabriel Aguiñaga Ruiz
Eliseo Ojeda Hernandez
