# TPE-BD2 - Proyecto con Python, Neo4j y MongoDB en GitHub Codespaces

Este repositorio contiene un proyecto de base de datos con Python, Neo4j y MongoDB, ejecutado a través de Jupyter Lab dentro de GitHub Codespaces.

---

## Requisitos del entorno

- Python (instalado automáticamente en Codespaces)
- Docker (configurado automáticamente en Codespaces)
- MongoDB y Neo4j deben estar corriendo como servicios (ver `data_load.ipynb` para detalles de conexión).
- Las dependencias de Python se instalan automáticamente desde `requirements.txt`.
---

## Iniciar en GitHub Codespaces

1. Hacer click en el botón verde **"Code"** en este repositorio.
2. Seleccionar **"Open with Codespaces"** y luego **"New codespace"**.
3. Esperar unos segundos a que se configure el entorno automáticamente (se construye usando el `Dockerfile` proporcionado en el repositorio).

---

## Iniciar Jupyter Lab

Una vez iniciado el Codespace:

1. En la terminal de VS Code (ya abierta por defecto), Jupyter Lab se inicia automáticamente gracias al `Dockerfile`.
2. Es importante asegurarse que la carpeta padre del proyecto es **TPE-BD2**.
3. Abrir el **puerto 8888** haciendo clic en el botón **"Ports"** en la parte inferior de Codespaces.
4. Buscar el puerto `8888` (estado: "Open in Browser") y hacer clic en "Open in Browser" (icono del mundo).

Esto abrirá Jupyter Lab en una pestaña del navegador.

---

## Usar los notebooks

1. En Jupyter Lab, abrir y ejecutar `data_load.ipynb` para cargar los datos necesarios.
2. Luego abrir y ejecutar `queries.ipynb` para realizar consultas sobre los datos.

---

## Notas

- No se requiere token ni contraseña para acceder a Jupyter Lab.
- Si el puerto 8888 no aparece, asegurarse de que el contenedor esté corriendo (`CMD` en el Dockerfile se encarga de eso).
- Si MongoDB o Neo4j no están conectando, revisar las URIs dentro de los notebooks.

---

