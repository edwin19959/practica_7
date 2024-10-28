# Usa una imagen de Python como base
FROM python:3.9-slim

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia los archivos de la aplicación a la carpeta /app en el contenedor
COPY . /app

# Instala Flask
RUN pip install flask

# Define la variable de entorno para Flask
ENV FLASK_APP=app.py

# Expone el puerto que Flask usará
EXPOSE 5000

# Comando para ejecutar la aplicación
CMD ["flask", "run", "--host=0.0.0.0"]
