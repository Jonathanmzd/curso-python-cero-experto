## Curso de FastAPI

### ¿Qué es FastAPI? con Sebastián Ramírez @Tiangolo

es un moderno y rápido marco (framework) web para construir APIs con Python 3.6+ basado en estándares y tipado de datos. Fue creado para ser fácil de usar y al mismo tiempo ofrecer alto rendimiento. Algunas de las características clave de FastAPI incluyen:

**Rápido y Eficiente:** FastAPI está diseñado para ser uno de los marcos web más rápidos disponibles para Python. Aprovecha la potencia de la anotación de tipos de datos para mejorar el rendimiento y también utiliza la biblioteca Starlette para manejar la capa de red.

**Tipado de Datos (Pydantic):** Utiliza anotaciones de tipos de datos para la validación y la documentación automática de la API. Además, se integra estrechamente con la biblioteca Pydantic, que facilita la validación y la serialización de datos de manera declarativa.

**APIs Autodocumentadas:** FastAPI genera automáticamente documentación interactiva (basada en Swagger y ReDoc) para tu API, lo que facilita a los desarrolladores comprender y probar la API sin necesidad de consultar la documentación por separado.

**Asíncrono por Defecto:** FastAPI es compatible con código asíncrono (async/await) de manera nativa, lo que permite manejar concurrencia de manera eficiente y aprovechar características avanzadas como WebSockets.

**Fácil Integración con Bibliotecas de Python:** Puedes integrar fácilmente FastAPI con otras bibliotecas populares de Python, como SQLAlchemy para el acceso a bases de datos, OAuth2 para la autenticación, y más.

**Seguridad Integrada:** FastAPI incluye características de seguridad integradas, como la validación y generación automática de esquemas OpenAPI, así como herramientas para manejar autorización y autenticación.

**Desarrollo Rápido (Rapid Development):** El marco está diseñado para facilitar el desarrollo rápido de aplicaciones, proporcionando características como la generación automática de código de cliente y la validación de datos de entrada y salida.

**Activo y en Desarrollo Continuo:** FastAPI es un proyecto activamente mantenido y actualizado. El creador del marco, Sebastián Ramírez, sigue agregando nuevas características y mejoras en cada versión.

En resumen, FastAPI es una opción poderosa y eficiente para construir APIs web con Python, especialmente si estás buscando un marco que combine velocidad, tipado de datos, documentación automática y soporte para programación asíncrona.


### Instalación de FastAPI y creación de tu primera aplicación

Instalar python en Windows 

![Alt text](image-1.png)

![Alt text](image.png)

![Alt text](image-2.png)

crear el entorno de python

```sh
python -m venv venv
```

Activar el entorno

```sh
venv/Scripts/activate
```

![Alt text](image-3.png)

Instalar depencias

```sh
pip install fastapi

pip install uvicorn
```

![Alt text](image-4.png)

levantar el servidor de la app

![Alt text](image-5.png)

```sh
uvicorn main:app --reload --port 5000 --host 0.0.0.0
```

**--host 0.0.0.0**  para que se muestre en red

![Alt text](image-6.png)

#### Recurso

https://github.com/platzi/curso-fastapi/tree/clase-01-creacion-aplicacion