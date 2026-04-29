# 🤝 Guía de Contribución

¡Gracias por tu interés en contribuir a **Elijo Quedarme**! Esta guía te ayudará a entender cómo participar en el proyecto.

## 📋 Proceso de Contribución

### 1. Fork el Repositorio
Haz clic en el botón "Fork" en la esquina superior derecha de GitHub para crear tu propia copia del proyecto.

### 2. Clona tu Fork
```bash
git clone https://github.com/tu-usuario/Talento_v2.git
cd Talento_v2
```

### 3. Crea una Rama
```bash
git checkout -b feature/tu-caracteristica
```

Usa nombres descriptivos:
- `feature/nueva-seccion` para nuevas características
- `fix/bug-description` para correcciones
- `docs/mejoras-documentacion` para documentación
- `style/mejoras-css` para cambios de estilo

### 4. Haz tus Cambios
Edita los archivos necesarios. Intenta mantener:
- Código limpio y comentado donde sea necesario
- CSS organizado y responsive
- JavaScript funcional y sin errores de consola
- Accesibilidad en mente (WCAG 2.1)

### 5. Commit de tus Cambios
```bash
git add .
git commit -m "Descripción clara del cambio"
```

Usa mensajes descriptivos:
- ✅ `Agregar formulario de contacto empresas`
- ✅ `Corregir animación en tarjetas de sellos`
- ❌ `cambio` 
- ❌ `arreglado`

### 6. Push a tu Fork
```bash
git push origin feature/tu-caracteristica
```

### 7. Crea un Pull Request
1. Ve a tu fork en GitHub
2. Haz clic en "Pull Request"
3. Describe tu cambio claramente
4. Espera feedback de los mantenedores

## 📝 Tipos de Contribuciones Bienvenidas

### 🐛 Reportar Bugs
Abre un Issue con:
- Descripción clara del problema
- Pasos para reproducir
- Comportamiento esperado
- Comportamiento actual
- Screenshots si es relevante
- Navegador/dispositivo usado

**Formato:**
```markdown
**Descripción del Bug:**
[Describe lo que pasó]

**Pasos para reproducir:**
1. 
2. 
3. 

**Resultado esperado:**
[Lo que debería pasar]

**Resultado actual:**
[Lo que pasó]

**Entorno:**
- Navegador: 
- SO: 
- Dispositivo:
```

### 💡 Sugerir Mejoras
Abre un Issue de Feature con:
- Descripción clara de la mejora
- Problema que resuelve
- Casos de uso
- Posibles implementaciones

### 📚 Mejorar Documentación
- Clarificar secciones confusas
- Agregar ejemplos
- Traducir a otros idiomas
- Corregir errores ortográficos
- Actualizar enlaces

### 🎨 Mejoras de Diseño/UX
- Propuestas de diseño
- Mejoras de accesibilidad
- Optimizaciones de rendimiento
- Mejoras en responsive design

### ✨ Nuevas Características
- Nuevas secciones
- Funcionalidades interactivas
- Integraciones
- Mejoras de flujo de usuario

## 🎨 Guías de Estilo

### CSS
- Usa variables CSS definidas en `:root`
- Mantén el código organizado por secciones
- Usa Flexbox/Grid para layouts
- Asegura responsive design con media queries
- Comenta código complejo

### JavaScript
- Usa nombres descriptivos para funciones y variables
- Comenta funcionalidades complejas
- Evita variables globales cuando sea posible
- Usa const/let en lugar de var
- Mantén funciones pequeñas y enfocadas

### HTML
- Usa etiquetas semánticas
- Asegura accesibilidad (alt text, labels, ARIA)
- Valida el HTML
- Indenta correctamente
- Comenta secciones principales

## 🔍 Antes de hacer Push

1. **Verifica tu código:**
   ```bash
   # Abre en navegador y prueba
   # Abre DevTools y revisa console
   # Prueba responsiveness
   ```

2. **Revisa cambios:**
   ```bash
   git diff
   ```

3. **Actualiza desde main:**
   ```bash
   git fetch origin
   git rebase origin/main
   ```

4. **Prueba en diferentes navegadores:**
   - Chrome/Edge
   - Firefox
   - Safari
   - Mobile browsers

## 📖 Estructura del Código

```
├── index.html          # Página de bienvenida
├── talento.html        # Página principal
├── README.md           # Documentación
├── package.json        # Metadata del proyecto
└── img/               # Imágenes (a agregar)
```

## 🚀 Roadmap del Proyecto

Prioridades actuales:
- [ ] Backend para persistencia de datos
- [ ] Sistema de auditoría de sellos
- [ ] Ranking dinámico
- [ ] Testimonios verificados
- [ ] Chat en vivo
- [ ] Notificaciones por email
- [ ] Dashboard administrativo

## 💬 Comunicación

- **Issues**: Para bugs y features
- **Discussions**: Para preguntas y conversaciones
- **Pull Requests**: Para contribuir código

## 📄 Código de Conducta

- Sé respetuoso
- Incluye a todos
- Crítica constructiva
- Sin spam o autopromoción
- Respeta la privacidad

## ✅ Checklist para PR

Antes de submitir tu Pull Request:

- [ ] Mi rama está actualizada con main
- [ ] Mi código sigue el estilo del proyecto
- [ ] He testeado mis cambios
- [ ] He actualizado la documentación si es necesario
- [ ] Mi commit tiene mensajes claros
- [ ] Sin errores en console
- [ ] Responsive en móvil, tablet y desktop
- [ ] Accesibilidad verificada

## 🎓 Recursos Útiles

- [Git Guide](https://git-scm.com/docs)
- [GitHub Docs](https://docs.github.com)
- [MDN Web Docs](https://developer.mozilla.org)
- [CSS Tricks](https://css-tricks.com)
- [A11y Checklist](https://www.a11yproject.com/checklist/)

## 🙏 Agradecimientos

¡Gracias por tu contribución! Cada aporte, sin importar el tamaño, ayuda a mejorar **Elijo Quedarme** y nuestra misión de retener talento en Aragón.

---

**¿Preguntas?** Abre una Discussion o contacta a los mantenedores.

¡Feliz contribuyendo! 🚀
