# Proyecto de Data Science con OpenWeatherMap API

Descripción general del proyecto y objetivos.

## Requisitos previos

- Docker
- Docker Compose
- WSL en Windows
- Python 3.x
- Cuenta en OpenWeatherMap y clave API

## Instrucciones de instalación y configuración

1. Clonar el repositorio:
```
git clone <URL_DEL_REPOSITORIO>
```

2. Crear y activar el entorno virtual de Python:
```
python3 -m venv venv
source venv/bin/activate  # En Linux/WSL
venv\Scripts\Activate  # En Windows
```

3. Instalar las dependencias del proyecto:
```
pip install -r requirements.txt
```

4. Configurar las variables de entorno necesarias (por ejemplo, claves API, credenciales de base de datos, etc.):
```
export OPENWEATHER_API_KEY=<TU_API_KEY>
```

## Ejecución del proyecto

1. Iniciar los contenedores Docker utilizando Docker Compose:
```
docker-compose up -d
```

2. Ejecutar los scripts de ETL para extraer, transformar y cargar datos desde la API de OpenWeatherMap:
```
python etl_script.py
```

3. Entrenar y evaluar el modelo de Machine Learning o Deep Learning:
```
python train_model.py
```

4. Acceder al dashboard de visualización:

- Si utilizas Data Studio, visita la URL del informe en tu navegador web.
- Si utilizas Streamlit, ejecuta el siguiente comando y visita la URL proporcionada en tu navegador web:
```
streamlit run app.py
```

## Detener y eliminar los contenedores Docker

Cuando desees detener y eliminar los contenedores Docker, ejecuta:
```
docker-compose down
```

## Contribuciones y soporte

Instrucciones para contribuir al proyecto o contactar al equipo de desarrollo para obtener soporte.