---

# 🚀 Proyecto Docker Compose con Nginx y Aplicaciones Web

## 📋 Descripción del Proyecto

Este proyecto utiliza **Docker Compose** para configurar un entorno con tres contenedores:

1. 🌐 **Proxy (Nginx)**: Actúa como proxy reverso y maneja las solicitudes en el puerto 80.
2. 🖥️ **Aplicación Web 1**: Servida en el contenedor `app1`.
3. 🖥️ **Aplicación Web 2**: Servida en el contenedor `app2`.

El proxy redirige las solicitudes a `/c2` y `/c3` hacia las aplicaciones web correspondientes.

## 🗂️ Estructura del Proyecto

```bash
proyecto-multicontenedor/
│
├── docker-compose.yml         # Archivo de configuración Docker Compose
├── nginx.conf                 # Configuración del proxy Nginx
├── welcome.html               # Página de bienvenida del proxy
├── Sintaxify/                 # Contenido de la Aplicación Web 1
│   └── index.html
└── AuthenticationServerFrontend/  # Contenido de la Aplicación Web 2
    └── index.html
```

## 🛠️ Instrucciones de Uso

### 1️⃣ Preparación del Entorno

1. **Crea el proyecto en tu máquina local**: Clona este repositorio o descarga los archivos necesarios.

2. **Verifica que Docker Compose esté instalado**: Puedes comprobarlo con el comando:

   ```bash
   docker-compose --version
   ```

### 2️⃣ Ejecución del Proyecto

1. **Navega al directorio del proyecto**:

   ```bash
   cd proyecto-multicontenedor
   ```

2. **Ejecuta el comando para iniciar los contenedores**:

   ```bash
   docker-compose up --build
   ```

   Este comando construirá y lanzará los contenedores definidos en el archivo `docker-compose.yml`.

### 3️⃣ Uso del Proyecto

1. **Abre tu navegador** y visita:

   - Página de bienvenida: [http://localhost:80](http://localhost:80)
   - Aplicación Web 1: [http://localhost/c2/](http://localhost/c2/)
   - Aplicación Web 2: [http://localhost/c3/](http://localhost/c3/)

## ✏️ Notas Adicionales

- Si estás utilizando **Play with Docker**, todos los comandos se ejecutan directamente en la terminal proporcionada por el servicio.
- Asegúrate de que los archivos `nginx.conf`, `welcome.html`, y los directorios `Sintaxify` y `AuthenticationServerFrontend` existan y estén correctamente configurados.

---
