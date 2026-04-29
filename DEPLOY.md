# 🚀 Guía de Deploy a GitHub

Esta guía te ayudará a subir el proyecto a GitHub y publicarlo en línea.

## 📋 Requisitos Previos

1. **Cuenta de GitHub** - [Crear aquí](https://github.com/signup)
2. **Git instalado** - [Descargar](https://git-scm.com/download)
3. **Terminal/CMD**
4. **Tu nombre de usuario de GitHub**

## 🔄 Paso 1: Crear un Repositorio en GitHub

1. Ve a https://github.com/new
2. Rellena los campos:
   - **Repository name**: `Talento_v2` (o tu preferencia)
   - **Description**: `Plataforma de certificación para retener talento joven en Aragón`
   - **Public** (para que sea visible)
   - **Initialize repository**: NO (ya tienes archivos locales)
3. Haz clic en "Create repository"
4. Copia la URL (ej: `https://github.com/tu-usuario/Talento_v2.git`)

## 🖥️ Paso 2: Configurar Git Localmente

```bash
# Abre terminal/CMD en la carpeta del proyecto
# Si estás en Windows, usa Git Bash

# Configura tu nombre y email
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@ejemplo.com"

# Verifica la configuración
git config --list
```

## 📤 Paso 3: Subir el Proyecto

```bash
# Navega a la carpeta del proyecto
cd C:\Users\tu-usuario\Desktop\Talento_v2

# Inicializa git (si no está ya inicializado)
git init

# Agrega todos los archivos
git add .

# Crea el primer commit
git commit -m "🚀 Initial commit: Plataforma Elijo Quedarme"

# Agrega el repositorio remoto (reemplaza URL)
git remote add origin https://github.com/TU-USUARIO/Talento_v2.git

# Sube al repositorio (main branch)
git branch -M main
git push -u origin main
```

## ✅ Paso 4: Verificar la Subida

1. Ve a tu repositorio en GitHub: `https://github.com/tu-usuario/Talento_v2`
2. Deberías ver:
   - ✅ Todos tus archivos
   - ✅ README.md visible
   - ✅ Commits en el historial

## 🌐 Paso 5: Activar GitHub Pages

1. En tu repositorio, ve a **Settings** (Configuración)
2. En la barra lateral, ve a **Pages**
3. En "Source", selecciona:
   - **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
4. Haz clic en "Save"
5. Espera 1-2 minutos

## 🎉 Paso 6: Acceder a tu Sitio

Tu sitio estará disponible en:
```
https://tu-usuario.github.io/Talento_v2/
```

- **Página de inicio**: `https://tu-usuario.github.io/Talento_v2/`
- **Plataforma principal**: `https://tu-usuario.github.io/Talento_v2/talento.html`

## 🔄 Paso 7: Hacer Cambios Futuros

Cada vez que quieras actualizar:

```bash
# Haz los cambios en tus archivos

# Agrega los cambios
git add .

# Crea un commit descriptivo
git commit -m "📝 Descripción del cambio"

# Sube los cambios
git push origin main

# GitHub Pages se actualiza automáticamente en 1-2 min
```

## 📝 Comandos Git Útiles

```bash
# Ver estado
git status

# Ver cambios
git diff

# Ver historial de commits
git log --oneline

# Deshacer último commit (sin perder cambios)
git reset --soft HEAD~1

# Ver ramas
git branch

# Crear nueva rama
git checkout -b feature/nombre

# Cambiar de rama
git checkout main

# Eliminar rama local
git branch -d nombre
```

## 🐛 Solución de Problemas

### "fatal: not a git repository"
```bash
git init
```

### "fatal: The current branch main has no upstream branch"
```bash
git push -u origin main
```

### "Permission denied (publickey)"
Configura tu SSH key o usa HTTPS en lugar de SSH:
```bash
git remote set-url origin https://github.com/tu-usuario/Talento_v2.git
```

### GitHub Pages no se actualiza
1. Ve a Settings → Pages
2. Verifica que Source esté en "Deploy from a branch"
3. Verifica que el branch es "main"
4. Espera 2-5 minutos

## 📱 Probar Antes de Subir

Antes de hacer push, prueba localmente:

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (si tienes http-server)
http-server
```

Luego abre: `http://localhost:8000`

## 🔐 Seguridad

### NO commits:
- ❌ Contraseñas
- ❌ API keys
- ❌ Tokens
- ❌ Información sensible

### Usa `.gitignore` para:
```
.env
*.key
secrets.json
node_modules/
```

## 📊 Agregar Información al Repositorio

### 1. Editar la descripción
1. Ve a Settings → General
2. Agrega una descripción breve
3. Agrega un tema (topic):
   - talento
   - aragón
   - empleo
   - educación

### 2. Agregar una Imagen de Perfil
1. Crea una imagen (recomendado 1:1)
2. Ve a Settings → Social preview
3. Sube la imagen

## 🎯 Próximos Pasos

1. **Colaboradores**: Ve a Settings → Collaborators y agrega a tu equipo
2. **Issues**: Crea una plantilla de issues
3. **Pull Requests**: Define qué se necesita en un PR
4. **Releases**: Crea releases para versiones principales
5. **Licencia**: Verifica que tengas LICENSE file (incluida en el repo)

## 📚 Recursos Adicionales

- [GitHub Docs](https://docs.github.com)
- [Git Cheat Sheet](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)
- [GitHub Pages Docs](https://pages.github.com/)
- [Markdown Guide](https://www.markdownguide.org/)

## 💡 Tips Pro

### Rama de desarrollo
```bash
# Crea rama para desarrollo
git checkout -b develop

# Haz cambios en develop
# Luego haz PR a main

# Esto mantiene main siempre funcional
```

### Ignorar archivos temporales
Agrega a `.gitignore`:
```
.DS_Store
Thumbs.db
*.swp
.vscode/
.idea/
```

### Mensajes de commit mejores
```
✅ ✨ Agregar formulario de contacto
🐛 🔧 Corregir layout en mobile
📚 📝 Actualizar documentación
🚀 🎨 Mejorar diseño de header
```

## ✨ ¡Listo!

Tu proyecto está en GitHub y publicado en línea. 

### Comparte:
- 📧 El enlace con tu equipo
- 🔗 Pégalo en tu CV/LinkedIn
- 🤝 Invita colaboradores
- ⭐ Haz que la gente le dé star

---

**¿Preguntas?** Revisa la documentación de GitHub o pregunta en los Discussions.

¡Felicidades por publicar tu proyecto! 🎉
