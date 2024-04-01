# Mi proyecto en Azure 

 # Aplicaciones/Creación de documentos/ Creación de aplicaciones de Azure/Autenticación con una Azure App/

[User Account](https://myaccount.microsoft.com/#) 
[@notebook-t.atlassian.net](https://notebook-t.atlassian.net/wiki/spaces/IS/Overview)  

[Avalonix module builders](https://myaccount.microsoft.com/groups/299e37d6-7446-47f4-a727-3c1da64d3414)



## Generación de un JWT

Aprende a crear un JSON Web Token (JWT) para autenticarte en determinados puntos de conexión de API REST con tu Azure App.

### Sobre JSON Web Token (JWT)

Para la autenticación como una aplicación o la generación de un token de acceso de instalación, debes generar un JSON Web Token (JWT). Si un punto de conexión de la API de REST necesita un JWT, la documentación de ese punto de conexión indicará que debes usar un JWT para acceder al punto de conexión.

El JWT debe estar firmado con el algoritmo RS256 y contener las siguientes notificaciones:

- `iat`: Emitido a las. Representa la hora a la que se creó el JWT. Para protegerte contra el desfase del reloj, se recomienda establecer este valor 60 segundos en el pasado y asegurarte de que la fecha y hora del servidor se establezcan con precisión (por ejemplo, mediante el Protocolo de hora de red).
- `exp`: Expira a las. Representa la hora de expiración del JWT, después de la cual no se puede usar para solicitar un token de instalación. El valor de tiempo debe ser máximo 10 minutos después.
- `iss`: Emisor. Representa el ID de tu Azure App. Este valor se usa para buscar la clave pública correcta para comprobar la firma del JWT. Puedes encontrar el ID de la aplicación utilizando el punto de conexión de la API de REST GET /app. Para obtener más información, consulta "Aplicaciones" en la documentación de la API de REST.
- `alg`: Algoritmo de código de autenticación de mensajes. Debería ser RS256, ya que el JWT debe firmarse mediante el algoritmo RS256.

Para usar un JWT, pásalo en el encabezado Authorization de una solicitud de API. Por ejemplo:

 
``` 
curl --request GET 
--url "https://api.azure.com/app" 
--header "Accept: application/vnd.azure+json" 
--header "Authorization: Bearer YOUR_JWT" 
--header "X-Azure-Api-Version: 2022-11-28"
 ```
 

En la mayoría de los casos, puedes usar `Authorization: Bearer` o `Authorization: token` para pasar un token. Sin embargo, si vas a pasar un token web JSON (JWT), debes usar `Authorization: Bearer`.

### Generación de un JSON Web Token (JWT)

La mayoría de los lenguajes de programación tienen un paquete que puede generar un JWT. En todos los casos, debes tener una clave privada y el ID de tu Azure App. Para obtener más información sobre cómo generar una clave privada, consulta "Administración de claves privadas para aplicaciones de Azure". Puedes encontrar el ID de la aplicación utilizando el punto de conexión de la API de REST GET /app. Para obtener más información, consulta "Aplicaciones" en la documentación de la API de REST.

Nota: En vez de crear un JWT, puedes usar los SDK de Octokit de Azure para autenticarte como aplicación. El SDK se encargará de generar un JWT automáticamente y volverá a generar el JWT una vez que expire el token. Para obtener más información, consulta "Scripting con la API de REST y JavaScript".

#### Ejemplo: Uso de Ruby para generar un JWT

Nota: Debes ejecutar `gem install jwt` para instalar el paquete jwt y poder usar este script.

En el siguiente ejemplo, reemplaza `YOUR_PATH_TO_PEM` por la ruta de acceso del archivo donde se almacena la clave privada. Reemplaza `YOUR_APP_ID` por el identificador de la aplicación. Asegúrate de poner los valores `YOUR_PATH_TO_PEM` y `YOUR_APP_ID` entre comillas dobles.

```ruby
require 'openssl'
require 'jwt'  # https://rubygems.org/gems/jwt
```

# Contenido de la clave privada

```
private_pem = File.read("YOUR_PATH_TO_PEM")
private_key = OpenSSL::PKey::RSA.new(private_pem)
```

# Genera el JWT

```
payload = {
  # Tiempo de emisión, 60 segundos en el pasado para tener en cuenta el desfase del reloj
  iat: Time.now.to_i - 60,
  # Tiempo de expiración del JWT (10 minutos máximo)
  exp: Time.now.to_i + (10 * 60),
  # Identificador de la Azure App
  iss: "YOUR_APP_ID"
}

jwt = JWT.encode(payload, private_key, "RS
```

## Descripción

Este proyecto es una aplicación web desarrollada utilizando las capacidades de Microsoft Azure. 
El propósito principal de utilizar Microsoft Azure como plataforma de nube es aprovechar sus servicios y capacidades para:

1. **Alojamiento en la Nube**: Proporcionar un entorno de alojamiento en la nube escalable y confiable para aplicaciones y servicios.

2. **Desarrollo y Despliegue de Aplicaciones**: Facilitar el desarrollo, prueba y despliegue de aplicaciones y servicios en la nube.

3. **Almacenamiento de Datos**: Almacenar y gestionar datos de manera segura y eficiente en la nube.

4. **Escalabilidad**: Permitir que las aplicaciones y recursos se escalen automáticamente según la demanda, lo que garantiza un rendimiento óptimo.

5. **Seguridad y Cumplimiento**: Ofrecer herramientas y características de seguridad avanzadas y ayudar a cumplir con regulaciones y estándares de seguridad.

6. **Análisis de Datos**: Facilitar el análisis de datos mediante servicios de inteligencia empresarial y aprendizaje automático.

7. **Internet de las Cosas (IoT)**: Admitir la conectividad y la gestión de dispositivos IoT.

8. **Integración Empresarial**: Permitir la integración de sistemas y servicios empresariales.

9. **Optimización de Costos**: Ayudar a optimizar los costos de infraestructura al pagar solo por los recursos utilizados.

10. **Continuidad del Negocio**: Ofrecer opciones de recuperación ante desastres y alta disponibilidad para garantizar la continuidad del negocio.

-----------------------------------------
## Tecnologías Utilizadas
-----------------------------------------
- Azure App Service
- Azure SQL Database
- Azure Functions

-----------------------------------------
## Configuración
-----------------------------------------
Asegúrate de configurar las siguientes variables de entorno:  

**AZURE_STORAGE_CONNECTION_STRING**: 
```
DefaultEndpointsProtocol=[protocolo];AccountName=[nombre de la cuenta];AccountKey=[clave de la cuenta];EndpointSuffix=[sufijo del punto de conexión]
```
----
**AZURE_DATABASE_CONNECTION_STRING**: 
```
Server=tcp:[nombre-del-servidor].database.windows.net;Database=[nombre-de-la-base-de-datos];User ID=[nombre-de-usuario];Password=[contraseña];Trusted_Connection=False;Encrypt=True;
```

-----------------------------------------
## Instalación
-----------------------------------------

Para ejecutar este proyecto localmente, sigue estos pasos: 

1. Clona este repositorio. 
2. [Instrucciones adicionales de instalación, si las hay.] 

-----------------------------------------
## Uso
-----------------------------------------
## Describe cómo usar tu proyecto aquí.
-----------------------------------------
## Contribuciones
-----------------------------------------
Si deseas contribuir a este proyecto, sigue los pasos: 

1. Fork este repositorio. 
2. Crea una rama para tu característica (`git checkout -b caracteristica-nueva`). 
3. Realiza tus cambios y haz commit (`git commit -m 'Añade característica nueva'`). 
4. Sube tus cambios (`git push origin caracteristica-nueva`). 
5. Abre una solicitud de extracción. 

-----------------------------------------
## Créditos 
-----------------------------------------

Este proyecto ha sido posible gracias al arduo trabajo y la colaboración de diversas personas y recursos. Queremos expresar nuestro agradecimiento a:

Equipo de Desarrollo:
- [Nombre del Desarrollador 1]
- [Nombre del Desarrollador 2]
- [Nombre del Desarrollador 3]

Diseño Gráfico:
- [Nombre del Diseñador Gráfico 1]
- [Nombre del Diseñador Gráfico 2]

Colaboradores Externos:
- [Nombre del Colaborador 1]
- [Nombre del Colaborador 2]

Agradecimientos Especiales:
- [Nombre de la Persona o Entidad Especial 1]
- [Nombre de la Persona o Entidad Especial 2]

Recursos y Herramientas Utilizados:
- [Nombre de la Herramienta 1]
- [Nombre de la Herramienta 2]

Agradecemos a todos los que han contribuido de alguna manera a este proyecto, ya sea a través de su tiempo, conocimientos o recursos. Sin su apoyo, este proyecto no habría sido posible.

¡Gracias a todos por ser parte de este logro!

Carlos Alberto Ibarra Perales 

-----------------------------------------
## Licencia 
-----------------------------------------

Este proyecto está bajo la licencia Linux GNU. 

-----------------------------------------
Consulta el archivo `LICENSE`  para obtener más detalles.
-----------------------------------------
