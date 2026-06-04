# 🛠️ Guía de Instalación de Python

## Windows

### Paso 1: Descargar Python
1. Ve a [python.org](https://www.python.org/downloads/)
2. Descarga Python 3.11+ (o la versión más reciente)
3. Ejecuta el instalador

### Paso 2: Configurar el instalador
- ✅ Marca: **Add Python to PATH** (IMPORTANTE)
- Selecciona: **Install Now** o **Customize Installation**
- Si personalizas, asegúrate de incluir pip

### Paso 3: Verificar instalación
Abre PowerShell o CMD y ejecuta:
```bash
python --version
pip --version
```
Deberías ver algo como: `Python 3.11.x` y `pip 23.x`

---

## macOS

### Opción 1: Con Homebrew (recomendado)
```bash
brew install python@3.11
```

### Opción 2: Desde python.org
1. Descarga el instalador macOS
2. Sigue las instrucciones
3. Verifica: `python3 --version`

---

## Linux (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install python3 python3-pip python3-venv
```

Verifica:
```bash
python3 --version
pip3 --version
```

---

## Configurar tu entorno de desarrollo

### 1. Instalar VS Code
- Descarga desde [code.visualstudio.com](https://code.visualstudio.com/)
- Instala la extensión: **Python** (Microsoft)

### 2. Crear un entorno virtual (recomendado)

```bash
# En el directorio del proyecto
python -m venv venv

# Activar entorno (Windows)
venv\Scripts\activate

# Activar entorno (macOS/Linux)
source venv/bin/activate
```

### 3. Instalar dependencias iniciales

```bash
pip install requests beautifulsoup4 paramiko cryptography
```

---

## Primeras pruebas

### Opción 1: Consola interactiva
```bash
python
```

Luego escribe:
```python
print("¡Hola, Python!")
```

### Opción 2: Crear un archivo

1. Crea un archivo `prueba.py`:
```python
print("¡Hola desde Python!")
print("¡Estoy listo para aprender!")
```

2. Ejecuta:
```bash
python prueba.py
```

---

## Troubleshooting

**Error: "python no es reconocido"**
- En Windows: Reinstala Python y asegúrate de marcar "Add Python to PATH"
- En Mac/Linux: Usa `python3` en lugar de `python`

**Error: "pip no encontrado"**
- Intenta: `python -m pip --version`
- Si falla: Reinstala Python incluyendo pip

---

¡Listo! Ya estás preparado para empezar el curso. 🚀
