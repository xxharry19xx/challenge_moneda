# challenge Convertidor de Monedas 

Este proyecto es una aplicación en Java que permite convertir montos entre diferentes monedas utilizando la API de ExchangeRate. Incluye un menú interactivo donde el usuario puede seleccionar la conversión deseada e ingresar el monto a convertir.

## Funcionalidades

- Conversión de:
  1. Dólar a Peso Argentino
  2. Peso Argentino a Dólar
  3. Dólar a Peso Colombiano
  4. Peso Colombiano a Dólar
  5. Dólar a Real Brasileño
  6. Real Brasileño a Dólar
- Salida del programa mediante la opción del menú.
- Cálculo dinámico basado en las tasas de cambio obtenidas de la API.

## Requisitos

- **Java 11 o superior**
- Conexión a Internet para acceder a la API de tasas de cambio

## Instalación

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   ```

2. Navega al directorio del proyecto:
   ```bash
   cd <NOMBRE_DEL_DIRECTORIO>
   ```

3. Asegúrate de que Maven está configurado y ejecuta el siguiente comando para descargar las dependencias:
   ```bash
   mvn clean install
   ```

## Uso

1. Ejecuta el archivo principal del proyecto:
   ```bash
   mvn exec:java -Dexec.mainClass="Main"
   ```

2. Selecciona una opción del menú interactivo y sigue las instrucciones para ingresar el monto a convertir.

3. El resultado de la conversión se mostrará en la consola.

## Librerías Utilizadas

- [Gson](https://github.com/google/gson): Para procesar el JSON recibido de la API.
- API ExchangeRate: Para obtener las tasas de cambio actualizadas.

## Estructura del Proyecto

```plaintext
src/
├── main/
│   ├── java/
│   │   ├── ExchangeRateClient.java   # Cliente para realizar solicitudes a la API
│   │   ├── ExchangeRateResponse.java # Modelo para mapear la respuesta de la API
│   │   └── Principal.java                 # Clase principal con el menú interactivo
│   └── resources/                    # Archivos de configuración (si aplica)
└── test/                             # Pruebas unitarias (pendiente de implementación)
```

## Ejemplo de Ejecución

```plaintext
=== Convertidor de Monedas ===
1. Dólar -> Peso Argentino
2. Peso Argentino -> Dólar
3. Dólar -> Peso Colombiano
4. Peso Colombiano -> Dólar
5. Dólar -> Real Brasileño
6. Real Brasileño -> Dólar
7. Salir
Seleccione una opción: 1
Ingrese el monto a convertir: 4
4.00 Dólares equivalen a 1398.00 Pesos Argentinos.
```

## Contribuciones

¡Las contribuciones son bienvenidas! Si deseas agregar nuevas funcionalidades o mejorar el código, siéntete libre de hacer un fork del repositorio y enviar un pull request.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

---

**Autor:** Harry Silva Vasquez
