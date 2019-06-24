## API REST

### Dependencias

Antes de compilar el proyecto asegurese de tener instalado lo siguiente:

* Java 8 JDK

* Maven (Apache Maven 3.3.9)

### Build & Deploy

Luego de descargar los achivos desde el repositorio dirijase a carpeta raiz del proyecto y ejecute el siguiente comando maven:


    $ mvn clean package
    
Para correr el programa asegurese de que el servicio Generador_Datos_Desafio_Uno esté corriendo en su máquina local y ejecute el siguiente comando:

    java -jar target/desafioRest-0.0.1-SNAPSHOT.jar


Nota: Debe estar disponible el puerto 9090 en el PC donde se ejecute esta solución

### Consumir Api

Para invocar el servicio debe ejecutar el siguiente comando

```bash
curl -X GET --header 'Accept: application/json' 'http://localhost:9090/service/ver01/periodos'
```

### Cocumentación del API

La documentación de swagger puede ser visualizada en la siguiente dirección:

http://localhost:9090/service/ver01/swagger-ui.html#/