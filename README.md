# Conexion-a-API-Gemini

Proyecto de integración con la API de Google Gemini utilizando Python y el SDK `google-genai`.

## Requisitos

Antes de comenzar, es necesario tener instalado:

- Python 3.13 o superior
- Git
- Una API Key de Google Gemini

## Instalación y ejecución

### 1. Clonar el repositorio

Abrir Git Bash y ejecutar:

```bash
git clone https://github.com/Ruzkyy/Conexion-a-API-Gemini.git
```

Entrar en la carpeta del proyecto:

```bash
cd Conexion-a-API-Gemini
```

### 2. Crear el entorno virtual

Crear un entorno virtual llamado `venv`:

```bash
python -m venv venv
```

Si el comando `python` no es reconocido, utilizar:

```bash
py -m venv venv
```

### 3. Activar el entorno virtual

En Git Bash:

```bash
source venv/Scripts/activate
```

Si la activación fue correcta, aparecerá `(venv)` al comienzo de la terminal.

### 4. Instalar las dependencias

Con el entorno virtual activado:

```bash
python -m pip install -r requirements.txt
```

Las principales dependencias utilizadas son:

- `google-genai`: conexión con la API de Gemini.
- `python-dotenv`: carga de variables de entorno.
- `requests`: solicitudes HTTP.

### 5. Configurar la API Key

Crear un archivo llamado `.env` en la raíz del proyecto:

```text
.env
```

Agregar la API Key:

```env
GEMINI_API_KEY=TU_API_KEY_AQUI
```

No subir el archivo `.env` a GitHub, ya que contiene información privada.

El archivo `.gitignore` está configurado para evitar que `.env` sea incluido en el repositorio.

## Ejecución

Una vez configurado el entorno virtual y las dependencias, ejecutar:

```bash
python mainGemini.py
```

Este programa realiza una solicitud a Gemini y muestra la respuesta generada por el modelo.

También se puede ejecutar el ejemplo de procesamiento de texto:

```bash
python app_text.py
```

Para comprobar que el entorno virtual y la conexión a Internet funcionan correctamente:

```bash
python main.py
```

## Estructura del proyecto

```text
Conexion-a-API-Gemini/
│
├── .env.example
├── .gitignore
├── README.md
├── requirements.txt
├── main.py
├── mainGemini.py
└── app_text.py
```

## Seguridad

La API Key debe mantenerse privada.

No subir al repositorio:

```text
.env
venv/
```

El archivo `.env.example` puede utilizarse como referencia para crear el archivo `.env` localmente.

## Flujo rápido

Si Python y Git ya están instalados, el proceso completo es:

```bash
git clone https://github.com/Ruzkyy/Conexion-a-API-Gemini.git
cd Conexion-a-API-Gemini
python -m venv venv
source venv/Scripts/activate
python -m pip install -r requirements.txt
python mainGemini.py
```
