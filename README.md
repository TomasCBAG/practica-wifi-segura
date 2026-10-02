# practica-wifi-segura

### Introducción ### 

En este informe estaremos realizando el análisis de un sitio web, estaremos buscando distintos tipos de riesgos, información sensible que no se encuentra cifrada, y explicaremos la mejora que se podrían tener 
implementando una VPN. Para finalizar daré tres reglas que bajo mi punto de vista son muy importantes


---Sitio analizado---
http://neverssl.com

// Protocolo utilizado //
El sitio utiliza el protocolo HTTP (HTTP/1.1), ya que la URL comienza con http:// y no con https://. Esto significa que la comunicación no utiliza el cifrado proporcionado por HTTPS.

* Host funfreshgrandspell.neverssl.com
* URL http://funfreshgrandspell.neverssl.com/online/
* Método GET
* User-Agent Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/154.0.0.0 Safari/537.36

Los riesgos de navegar en una red WiFi publica mediante HTTP

Al utilizar HTTP, la información transmitida no está protegida mediante cifrado HTTPS. En una red Wi-Fi pública, un atacante que pueda interceptar el tráfico podría observar información transmitida durante la comunicación. Por eso HTTPS es importante para proteger la confidencialidad e integridad de los datos.


----Uso de VPN----
Una VPN crea un túnel seguro y cifrado entre el dispositivo y el servidor VPN. Esto ayuda a proteger el tráfico, especialmente cuando se utiliza una red Wi-Fi pública, porque dificulta que otras personas de la misma red puedan observar los datos transmitidos. También proporciona mayor privacidad al ocultar la dirección IP del usuario frente a los sitios que visita, aunque la VPN no convierte por sí sola una conexión HTTP en HTTPS.
Cifrado: protege los datos dentro del túnel VPN.
Túnel seguro: establece una conexión protegida con el servidor VPN.
Protección del tráfico: dificulta la interceptación del tráfico en la red local.
Privacidad: el sitio puede ver la IP del servidor VPN en lugar de la IP pública del usuario.

!! 3 reglas de Oro !!!
Evitar ingresar información sensible (contraseñas, datos bancarios, etc.) en sitios que no utilicen HTTPS.
Utilizar una VPN cuando sea necesario conectarse a una red Wi-Fi pública.
Desactivar la conexión automática a redes Wi-Fi públicas y conectarse únicamente a redes conocidas y confiables.
