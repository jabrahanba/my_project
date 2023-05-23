# Dockerfile-jupyter

# Utilizar imagen base oficial de Jupyter Notebook
FROM jupyter/base-notebook

# Instalar las bibliotecas necesarias
COPY requirements.txt /tmp/
RUN pip install --requirement /tmp/requirements.txt

# Copiar los notebooks del proyecto al directorio de trabajo
COPY notebooks/ /home/jovyan/

# Exponer el puerto de Jupyter Notebook
EXPOSE 8888
