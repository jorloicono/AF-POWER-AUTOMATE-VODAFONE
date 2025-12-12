# Introducción a Power Automate y NoCode

## Relación con Microsoft 365
Power Automate permite crear flujos automatizados dentro del entorno Microsoft 365, integrándose fácilmente con:
- **Excel**  
- **Teams**  
- **OneDrive**  
- **Forms**  
- **Power BI**

---

## Tipos de flujo
- **Flujo automático**: se ejecuta cuando ocurre un evento (ej. “cuando se recibe un correo”).  
- **Flujo instantáneo**: se ejecuta manualmente mediante un botón.  
- **Flujo programado**: se ejecuta en intervalos o horarios definidos.  

También pueden utilizarse **plantillas recomendadas** para comenzar rápidamente.

---

## Conectores clave
- **Outlook**
- **Teams**
- **OneDrive / SharePoint**
- **Forms**
- **Excel Online**

---

## Crear un flujo desde cero
Pasos generales:
1. Elegir un **disparador**, por ejemplo:
   - Correo recibido en Outlook  
   - Envío de una respuesta de Forms  
   - Archivo creado o modificado en OneDrive o SharePoint  
2. Añadir acciones según la lógica deseada.  
3. Guardar y probar el flujo.

---

## Contenido dinámico básico
Uso de información proveniente del disparador o de acciones previas:
- Campos del **correo** (remitente, asunto, cuerpo)  
- **Metadatos de archivos** (nombre, ruta, creador, fecha)

## Condiciones sencillas (IF/ELSE)
Las **condiciones** permiten tomar decisiones dentro del flujo según valores dinámicos.  
Funcionamiento básico:
1. Agregar acción **"Condición"**.
2. Definir una regla, por ejemplo:  
   - *Si el asunto del correo contiene "urgente"*  
   - *Si la respuesta del formulario es igual a "Sí"*  
3. Configurar las ramas:  
   - **Si verdadero**: ejecutar las acciones correspondientes.  
   - **Si falso**: realizar acciones alternativas o dejar vacío.

Ejemplos típicos:
- Clasificar correos en carpetas según palabras clave.  
- Enviar notificaciones solo si una respuesta cumple cierto criterio.  
- Mover archivos a carpetas distintas según su tipo.

---

## Supervisión básica del flujo

### Historial de ejecuciones
Desde la sección **Mis flujos**, cada flujo muestra:
- **Ejecuciones recientes**  
- Estado: *Correcto*, *Error* o *Cancelado*  
- Entrada/salida de cada acción

Esto permite identificar rápidamente dónde falló un proceso.

### Errores más frecuentes
- Conectores sin autenticación o credenciales caducadas.  
- Archivos o rutas que ya no existen.  
- Esperar un tipo de dato incorrecto en condiciones o expresiones.  
- Falta de permisos en SharePoint, Teams o OneDrive.

### Activación / Desactivación del flujo
- Cada flujo puede **activarse o desactivarse** desde su menú.  
- Útil para pausar automatizaciones mientras se realizan pruebas o cambios.  
- Al desactivarlo, no se ejecutará ni aunque se dispare el evento.


- **Respuestas de formulario** (preguntas y valores enviados)  
```
