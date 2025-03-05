# BTLO-Phishing Analysis

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image.png)

En este laboratorio de Blue Team Labs Online, hemos recibido un correo electrónico de phishing reenviado por un usuario al SOC. El objetivo es investigar el correo y su archivo adjunto para recopilar información útil y detectar posibles amenazas.

Usaremos **Editor de Texto** para revisar los encabezados del correo, el remitente y los enlaces incluidos en el mensaje. Esto nos permitirá verificar si el correo proviene de una fuente confiable o si contiene señales de falsificación. También utilizaremos **URL2PNG** para capturar vistas previas de los enlaces sospechosos y analizar si apuntan a sitios maliciosos. Además, realizaremos una consulta **WHOIS** sobre los dominios relacionados para identificar registros de dominios sospechosos.

En caso de que el archivo adjunto contenga malware, realizaremos un análisis detallado en un entorno seguro. Al final, se proporcionarán recomendaciones sobre cómo prevenir futuros ataques de phishing, incluyendo el bloqueo de direcciones sospechosas y la educación de los usuarios para evitar caer en este tipo de engaños.

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%201.png)

### Enunciado:

Un usuario recibió un correo electrónico de phishing y lo reenvió al SOC. ¿Puede investigar el correo electrónico y el archivo adjunto para recopilar información útil?

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%202.png)

==============================================================

### **Nota:** Este laboratorio lo resolveremos en Windows, no usaremos comandos , solo analizaremos el phising.

==============================================================

**PRIMEROS PASOS:**

Procedemos a descargar y descompimir el archivo:

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%203.png)

Nos pedira la contraseña y esta es : btlo

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%204.png)

Luego abriremos el archivo con Editor de Texto, tambien lo abriremos con Outlook.

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%205.png)

## RESPONDAMOS:

### 1.¿Quién es el destinatario principal de este correo electrónico?

Buscamos el destinatario: Podemos buscar mas rapidamente entrando en Edicion y luego en Buscar, o tambien haciendo Ctrl + B :

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%206.png)

**Respuesta:** kinnar1975@yahoo.co.uk 

### 2.¿Cuál es el asunto de este correo electrónico?

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%207.png)

**Respuesta :** Undeliverable: Website contact form submission

### 3.¿Cuál es la fecha y hora en que se envió el correo electrónico?

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%208.png)

**Respuesta:** 18 March 2021 04:14

### 4.¿Cuál es la IP de origen?

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%209.png)

**Respuesta:** 103.9.171.10

### 5.Realizar DNS inverso en esta dirección IP, ¿cuál es el host resuelto? ([whois.domaintools.com](http://whois.domaintools.com/))

**Domaintools:** es una plataforma que recopila datos de dominios, sitios web y DNS para ofrecer análisis de riesgos y contexto inmediato.

Para responder esta pregunta, entramos a  [whois.domaintools.com](http://whois.domaintools.com/) y pegaremos la IP:

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%2010.png)

Tambien lo podemos encontrar en el Editor de Texto

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%2011.png)

**Respuesta:** c5s2-1e-syd.hosting-services.net.au

### 6.¿Cómo se llama el archivo adjunto?

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%2012.png)

**Respuesta:** Website contact form submission.email

### 7.¿Cuál es la URL que se encuentra dentro del archivo adjunto?

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%2013.png)

**Respuesta:** 

https://35000usdperwwekpodf.blogspot.sg?p=3D9swghttps://35000usdperww=ekpodf.blogspot.co.il?o=3D0hnd

### 8.¿En qué servicio está alojada esta página web?

De la URL podemos observar el servicio:

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%2014.png)

**Respuesta:** blogspot

### 9.Usando URL2PNG, ¿cuál es el texto del encabezado de esta página? (¡No importa si la página ha sido eliminada!)

URL2PNG: Es un servicio que permite a las empresas en línea capturar capturas de pantalla de páginas web y convertirlas en archivos de imagen

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%2015.png)

Respuesta: Blog has been removed

### **Felicidades, completaste todas las respuestas**

![](https://github.com/EnocRosales20/Writeup_BTLO_Physing_Analysis/blob/main/images/image%2016.png)
