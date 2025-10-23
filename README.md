# 🧠 Proyecto Saber Pro IA - Tutor Virtual UDC

## 📘 Descripción General
Este repositorio contiene el desarrollo completo del **Tutor Virtual para la preparación Saber Pro**, una solución basada en **Inteligencia Artificial** que asiste a los estudiantes en la preparación de la prueba mediante simulaciones, análisis de desempeño y retroalimentación inteligente.

El proyecto integra módulos de interfaz, lógica de tutoría, bases de datos y archivos de soporte (.zip, .rar) gestionados mediante **Git Large File Storage (LFS)** para un manejo eficiente de archivos grandes.

---

## 🧩 Requisitos Previos

Antes de comenzar, asegúrate de tener instaladas las siguientes herramientas:

| Herramienta | Descripción | Verificación |
|--------------|-------------|---------------|
| [Git](https://git-scm.com/) | Control de versiones | `git --version` |
| [Git LFS](https://git-lfs.com/) | Manejo de archivos grandes | `git lfs version` |
| [Visual Studio Code](https://code.visualstudio.com/) | Entorno de desarrollo | `code --version` |
| [Python](https://www.python.org/) *(si aplica)* | Entorno backend o IA | `python --version` |
| [Node.js / npm](https://nodejs.org/) *(si aplica)* | Entorno frontend | `node -v` / `npm -v` |

---

## 🚀 Guía Completa de Clonado y Despliegue

### 🔹 Paso 1: Clonar el Repositorio desde GitHub

Abre tu **terminal (CMD o PowerShell)** y ejecuta:

```bash
git clone https://github.com/AlejoTechEngineer/Proyecto_Saber_Pro_IA_Tutor_Virtual_UDC.git
cd Proyecto_Saber_Pro_IA_Tutor_Virtual_UDC
```

---

### 🔹 Paso 2: Configurar Git LFS

Antes de abrir el proyecto, descarga correctamente los archivos grandes:

```bash
git lfs install
git lfs pull
```

Esto asegura que los archivos `.zip` y `.rar` se descarguen completos.

---

### 🔹 Paso 3: Abrir el Proyecto en Visual Studio Code

```bash
code .
```

O manualmente:
1. Abre **Visual Studio Code**
2. Selecciona **Archivo → Abrir carpeta**
3. Elige la carpeta clonada del proyecto

---

### 🔹 Paso 4: Instalar Dependencias

Dependiendo del módulo que ejecutes:

**Si es un proyecto Node.js:**
```bash
npm install
```

**Si es un proyecto Python:**
```bash
pip install -r requirements.txt
```

---

### 🔹 Paso 5: Ejecutar el Proyecto

**En Node.js:**
```bash
npm start
```

**En Python (Flask o FastAPI):**
```bash
python app.py
```

---

### 🔹 Paso 6: Visualizar el Proyecto

Una vez iniciado el servidor local, abre tu navegador en:

- Node.js → [http://localhost:3000](http://localhost:3000)  
- Python → [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 🗂️ Estructura del Proyecto

```
Proyecto_Saber_Pro_IA_Tutor_Virtual_UDC/
│
├── DATA SABER PRO UTIL/
│   └── Saber Pro S.rar
│
├── Tutor Virtual Codigo/
│   └── TutorVirtual-main.zip
│
├── assets/
│   └── recursos estáticos (imágenes, íconos, etc.)
│
├── docs/
│   └── documentación técnica y guías
│
├── README.md
└── .gitattributes
```

---

## 💾 Actualización del Repositorio

Para mantener tu versión local actualizada con la versión remota:

```bash
git pull origin main
git lfs pull
```

---

## ⚙️ Resolución de Problemas Comunes

### ❌ Error: “File exceeds 100MB”
➡ Esto ocurre si Git LFS no está activo.  
Solución:
```bash
git lfs install
git lfs track "*.zip"
git lfs track "*.rar"
git add .gitattributes
git commit -m "Activar LFS para archivos grandes"
git push origin main
```

---

### ❌ Error: No se instalan dependencias
Si al ejecutar `npm start` o `python app.py` aparecen errores, reinstala dependencias:

```bash
npm install
```
o  
```bash
pip install -r requirements.txt
```

---

### ❌ El servidor no arranca
Verifica que el puerto esté libre:
```bash
npx kill-port 3000
```
Y luego vuelve a ejecutar:
```bash
npm start
```

---

## 👨‍💻 Autor

**Alejandro De Mendoza Tovar**  
_Universitaria de Colombia_  
**GitHub:** [AlejoTechEngineer](https://github.com/AlejoTechEngineer)

---

## 📄 Licencia

**Licencia MIT** — Uso educativo y no comercial permitido con atribución.  
Puedes modificar, distribuir y utilizar el código con fines académicos bajo esta licencia.

---

> **Repositorio oficial:**  
> 🔗 [https://github.com/AlejoTechEngineer/Proyecto_Saber_Pro_IA_Tutor_Virtual_UDC](https://github.com/AlejoTechEngineer/Proyecto_Saber_Pro_IA_Tutor_Virtual_UDC)
