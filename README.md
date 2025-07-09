# Proyecto CI/CD con GitHub Actions y Vercel

Este proyecto es una demostración práctica del uso de **Integración y Entrega Continua (CI/CD)** utilizando **GitHub Actions** para la automatización del flujo de trabajo y **Vercel** como plataforma de despliegue.

---

## 🔧 Estructura del proyecto

- `index.html`: Archivo principal del sitio web.
- `.github/workflows/deploy.yml`: Archivo de configuración del workflow de GitHub Actions.
- `README.md`: Documento explicativo del proyecto y su implementación CI/CD.

---

## 🚀 ¿Qué hace este proyecto?

1. Cada vez que se realiza un cambio en la rama `main` y se hace push:
2. GitHub Actions ejecuta un workflow automático (definido en `deploy.yml`).
3. Vercel detecta el cambio y genera un nuevo despliegue del sitio web automáticamente.

---

## ⚙️ CI/CD - GitHub Actions

El archivo `deploy.yml` incluye:

- **Checkout del repositorio**  
  Usando `actions/checkout@v3`.

- **Instalación de dependencias**  
  (No se requería para este proyecto HTML estático).

- **Ejecución de pruebas**  
  No aplicaba en este caso.

- **Despliegue a Vercel**  
  Vercel detecta automáticamente los cambios al hacer push en GitHub.

---

## 🌐 Despliegue en Vercel

El sitio fue desplegado automáticamente mediante integración con [Vercel](https://vercel.com).

**URL del sitio desplegado:**  
[https://ci-cd-github-actions-gray.vercel.app](https://ci-cd-github-actions-gray.vercel.app)


> *(Reemplaza <TU-NOMBRE> por la URL real de tu sitio si ya lo tienes desplegado.)*

---

## 👩‍💻 Comandos utilizados

```bash
git init
git remote add origin https://github.com/Karen2431-oss/ci-cd-github-actions.git
git add .
git commit -m "Primer commit"
git push -u origin main
