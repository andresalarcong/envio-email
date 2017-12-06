# envio-email

* Se usa el patrón PageObject.
* Se usó una arquitectura de tres capas (Negocio y Definición, SubFlujos o
comportamientos de negocio, Representación e interacción directa con los
elementos a probar), gracias a Serenity BDD.
* Uso de XPath para la búsqueda de elementos en el DOM.
* Usa gradle.
* Se usa Test Data Driven.
* Puede ejecutarse en cualquier sistema operativo de cualquier arquitectura
de hardware por sus condiciones (No embebe un ejecutable de driver de
navegador gracias a Selenium 3 y usa Java que se ejecuta en la mayoría de
arquitecturas). Recuerda ingresar al path del sistema operativo el driver.
* Se hace una simple instrumentación de código, con Logger.
* Se usa Gherkin al idioma español y en los reportes también.
* Se realiza una prueba unitaria a modo de ejemplo sobre la instanciación del driver que se encarga de ejecutar las
acciones con el navegador web.
* Está listo para pegarse a un servidor de integración continua que soporte
gradle.
* Usa Cucumber por lo que ayuda a tener un código más limpio, por ejemplo
usa un mapeo de objetos desde el gherkin a objetos Java directamente.

Recuerda usar la propiedad F.I.R.S.T en las pruebad.


Para ejecutar el script instala gradle en el sistema operativo y agrega al path de las variables del sistema operativo

1. gradle wrapper - Si el proyecto no tiene la carpeta /gradle/wrapper o si deseas generarlo en tu maquina (opcion recomendada) Para ello borra la carpeta gradle, gradlew y gradle.bat y ejecuta lo siguiente: gradle wrapper (Si se presenta errores de gradle configura la versión 4)
2. gradlew clean test aggregate '-Dwebdriver.driver=chrome' (o el navegador que quieras, recuerda que requieres agregar al path el driver)

Recuerda crearte tu correo remitente y destinatario en gmail.

Requisitos:
  * Java JDK 1.8u131 en adelante.
  * ChromeDriver en las variables del sistema versión 2.33 (Donde se ejecutará la suite de pruebas)
  * Gradle 4 en adelante en las variables de sistema.
  
  
