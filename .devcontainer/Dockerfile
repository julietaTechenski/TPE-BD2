FROM python:3.11

# Instalar dependencias del sistema
RUN apt-get update && apt-get install -y curl && apt-get clean

# Instalar Python packages
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Crear carpeta para notebooks
RUN mkdir -p /home/jovyan/work
WORKDIR /home/jovyan/work

# Comando por defecto: iniciar Jupyter
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--allow-root", "--NotebookApp.token=''", "--NotebookApp.password=''"]
