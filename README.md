# 💱 Conversor de Monedas en Java

Este proyecto es una aplicación de consola en Java que permite convertir valores entre diferentes monedas utilizando tasas de cambio obtenidas en tiempo real desde una API pública.

## Acerca del Proyecto

Este conversor de monedas fue desarrollado como parte del desafío académico para la Escuela Alura LATAM,En la formacion (java orientado a objectos, G8-ONE) dentro del programa Oracle Next Education. El objetivo principal es aplicar los conocimientos de Java para interactuar con APIs externas, manejar respuestas JSON y desarrollar una aplicación de consola funcional y bien estructurada.

El autor del proyecto es **Alexander Restrepo Epieyu mas ayuda academica**.

El programa realiza consultas a la API "Exchange Rate API" para obtener las tasas de cambio más recientes. Utiliza `java.net.http.HttpClient` para las peticiones HTTP y la biblioteca Gson para el procesamiento eficiente de los datos en formato JSON. El código está desarrollado en Java 17, buscando seguir principios de responsabilidad única por clase.

## ✨ Características

* Conversión de monedas en tiempo real.
* Interfaz de usuario interactiva a través de la consola.
* Uso de tasas de cambio actualizadas desde una API externa.

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Java 17.
* **Cliente HTTP:** `java.net.http.HttpClient` (Módulo `java.net.http`)
* **Procesamiento JSON:** [Gson](https://github.com/google/gson)
* **API de Tasas de Cambio:** [Exchange Rate API](https://www.exchangerate-api.com/)

## 📋 Prerrequisitos

Antes de comenzar, asegúrate de tener instalado lo siguiente:

* **Java Development Kit (JDK):** Versión 17 o superior.
* **Git:** Para clonar el repositorio.
* **API Key de Exchange Rate API:** Necesitarás registrarte para obtener una clave gratuita.
* **Acceso a Internet:** Para que la aplicación pueda consultar la API.
* **Biblioteca Gson:** Asegúrate de que la biblioteca Gson esté disponible en tu classpath. Si no utilizas un gestor de dependencias como Maven o Gradle, deberás descargar el archivo `.jar` de Gson y añadirlo manualmente a tu proyecto/classpath.

## 🚀 Instalación y Configuración

Sigue estos pasos para poner en funcionamiento el conversor de monedas:

1.  **Clonar el Repositorio:**
    ```bash
    git clone https://URL_DE_TU_REPOSITORIO_AQUI.git
    cd nombre-del-directorio-del-proyecto
    ```
    *(Reemplaza `https://URL_DE_TU_REPOSITORIO_AQUI.git` con la URL real de tu repositorio y `nombre-del-directorio-del-proyecto` con el nombre de la carpeta del proyecto).*

2.  **Configurar la API Key (MUY IMPORTANTE):**
    Este proyecto requiere una API key de [Exchange Rate API](https://www.exchangerate-api.com/) para funcionar.

    * **Obtén tu API Key:** No necesitas registrarte para obtener una clave gratuita en [www.exchangerate-api.com](https://www.exchangerate-api.com/).

## 💻 Uso

1.  **Ejecutar la Aplicación:**
    * **Desde un IDE (Recomendado):** Abre el proyecto en tu entorno de desarrollo integrado (como IntelliJ IDEA, Eclipse, NetBeans). Localiza y ejecuta la clase principal 
    Al iniciar la aplicación, se te presentará un menú similar a este:

    ```
    ******************************************************
    Sea bienvenido/a al Conversor de Monedas =]

    Elija una opción de conversión:
    1) Dólar (USD) => Peso Argentino (ARS)
    2) Peso Argentino (ARS) => Dólar (USD)
    3) Dólar (USD) => Real Brasileño (BRL)
    4) Real Brasileño (BRL) => Dólar (USD)
    5) Dólar (USD) => Peso Colombiano (COP)
    6) Peso Colombiano (COP) => Dólar (USD)
    7) Salir

    Por favor, elija una opción válida:
    ******************************************************
    ```
    * Ingresa el número de la opción de conversión que deseas realizar y presiona `Enter`.
    * A continuación, el programa te solicitará que ingreses la cantidad de dinero que deseas convertir. Escríbela y presiona `Enter`.
    * El resultado de la conversión, utilizando la tasa de cambio actual, se mostrará en pantalla.

    **Ejemplo de Interacción:**
    ```
    Por favor, elija una opción válida: 1
    Ingrese la cantidad que desea convertir de USD a ARS: 100
    El valor de 100.00 [USD] corresponde al valor final de =>>> XXX.XX [ARS]
    ```
    *(El valor XXX.XX dependerá de la tasa de cambio en el momento de la consulta).*

## 📂 Estructura del Proyecto (Ejemplo)

Una posible estructura de clases podría ser:

* `Principal.java`: Clase principal que contiene el método `main` y maneja el menú y la interacción con el usuario.
* `ConsultaMoneda.java` (o `ApiConnector.java`): Clase responsable de realizar las consultas a la API de Exchange Rate.
* `Moneda.java` (o `ConversionRate.java`): Clase (record o regular) para mapear la respuesta JSON de la API.
* `GeneradorDeArchivo.java` (si aplica): Clase para guardar historial de conversiones (si esta funcionalidad existe).
* Otras clases de modelo o utilidad según sea necesario.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar este proyecto:

1.  Haz un Fork del repositorio.
2.  Crea una nueva rama para tu característica o corrección (`git checkout -b feature/NuevaCaracteristica` o `fix/CorreccionError`).
3.  Realiza tus cambios y haz commit (`git commit -m 'Añade NuevaCaracteristica'`).
4.  Haz Push a tu rama (`git push origin feature/NuevaCaracteristica`).
5.  Abre un Pull Request.

## 📄 Licencia

Este proyecto se distribuye bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
*(Deberás crear un archivo `LICENSE` en la raíz de tu repositorio con el texto de la Licencia MIT).*

## 🧑‍💻 Autor y Agradecimientos

* **Autor:** Alexander Restrepo Epieyu
* **GitHub:** [TuPerfilDeGitHub](https://github.com/tu_usuario_aqui) *(Reemplaza con tu enlace)*

Este proyecto fue desarrollado como un desafío dentro del programa **Oracle Next Education (ONE)** en colaboración con **Alura LATAM**.

---
¡Esperamos que este conversor de monedas te sea útil!
