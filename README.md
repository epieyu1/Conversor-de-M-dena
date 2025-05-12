*** Conversor de Monedas en Consola ***

Este es un sencillo programa de consola en Java que permite a los usuarios convertir montos ya definidos, entre diferentes monedas utilizando tasas de cambio obtenidas en tiempo real desde una API externa, "exchangerate-api.com".

## Descripción General

El programa presenta un menú interactivo donde el usuario puede seleccionar el par de monedas para la conversión (por ejemplo, Dólar a Peso Argentino, Peso Argentino a Dólar, etc.) e ingresar el monto que desea convertir. Luego, la aplicación se conecta a la API de "exchangerate-api.com" para obtener la tasa de cambio más reciente y calcula el monto convertido, mostrando tanto la tasa como el resultado final.

## Características ##

 * Menú Interactivo:** Interfaz de usuario basada en texto fácil de usar.
 * Múltiples Pares de Monedas: Soporta conversiones predefinidas:
 
    === Conversor de Monedas ===
    
    1: Dólar => Peso Argentino
    2: Peso argentino => Dolar
    3: Dólar => Real Brasileño 
    4: Real Brasileño => Dolar
    5: Dólar => Peso Colombiano
    6: Peso Colombiano => Dolar
    7: Salir
    
 * Tasas de Cambio en Tiempo Real: Utiliza la API `v6.exchangerate-api.com` para obtener datos actualizados.
 * Cálculo de Conversión:** Muestra la tasa de cambio aplicada y el monto resultante.
 * Formato de Salida Claro:** Los resultados numéricos se presentan con formato para facilitar la lectura.

*** Prerrequisitos ***

_ Java Development Kit (JDK):** Versión 17 u otro.
_ Conexión a Internet:** Necesaria para que la aplicación pueda acceder a la API de tasas de cambio.

*** Tecnologías Utilizadas ***
- Java (JDK 17 u otra version)
- Gson (para manejo de JSON)
- HttpClient (para solicitudes HTTP)
- Exchange Rate API

1. Clona este repositorio o descarga el archivo (.java).
2. Descarga y agrega la librería [Gson 2.13.1](https://repo1.maven.org/maven2/com/google/code/gson/gson/2.13.1/).
3. Regístrate en [ExchangeRate-API](https://www.exchangerate-api.com/) y obtén tu API key.
4. Sustituye la API key en el código:  
   
   String url = "https://v6.exchangerate-api.com/v6/TU_API_KEY/pair/" + base + "/" + destino + "/" + monto;

*** Ejemplo de Uso ***

=== Conversor de Monedas ===
1. Dólar => Peso argentino
 
Selecciona una opción: 1
2. Ingresa el monto a convertir: 100

=== Resultado de Conversión ===
De: USD → A: ARS
Tasa: 1 USD = 900.50 ARS
Resultado: 100 USD = 90,050.00 ARS

Autor
Desarrollado por Alexander Restrepo Epieyu, mas Ayuda acamedica.

Licencia
Este proyecto está bajo la Licencia MIT. Puedes usarlo, modificarlo y distribuirlo libremente.

