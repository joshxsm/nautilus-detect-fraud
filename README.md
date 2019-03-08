# nautilus-detect-fraud
Prototype bot to detect fraud in wallapop.es

Un sistema prototipo de un bot en python / php que detecta fraude y contenido fraudulento “in-live” a todas la conversaciones iniciadas para los nuevos productos, por ejemplo:




* Factores que analizaría el bot como palabras claves y saltaría una validación o aviso de análisis de fraude para que el usuario tenga cuidado.
* Fecha de creación de la cuenta
* Análisis de creación de usuario (Social / Email -> verificar si es un mail temporal o falso a través de una blacklist)
* Sin avatar 
* Estado de verificación de la cuenta
* Sin valoraciones
* Productos vendidos / comprados < 0
* Sin localización
* Que en el primer mensaje solicite contactar por WhatsApp si aparece la palabra clave como “WhatsApp o una numeración telefónica ( nacional o internacional)
* Si después de los primeros mensajes del usuario y de haberle avisado el comprador no envía mensajes en un periodo de 72h recomiendo añadirlo a una lista negra interna en wallapop con los mails que ha creado esa cuenta , ip, localización, id social, etc…
 * Si el bot tiene dudas o se encuentra con incongruencias se le notificara al equipo de soporte para que analice el caso con autorización del usuario.
