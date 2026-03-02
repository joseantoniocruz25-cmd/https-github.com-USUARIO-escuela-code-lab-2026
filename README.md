# 🎓 Escuela Code Lab 2026

Plataforma interactiva de ejercicios prácticos de JavaScript y CSS para estudiantes, con **código completamente comentado en español** como guía de estudio.

## 📋 Descripción

Este proyecto contiene una colección de **12 ejercicios prácticos** organizados en sesiones progresivas, diseñados para enseñar desarrollo web frontend desde los fundamentos hasta técnicas avanzadas de WebGL y animaciones. Cada ejercicio incluye comentarios educativos detallados que explican **QUÉ** hace el código, **POR QUÉ** es importante y **CÓMO** funciona.

## ✨ Características

- 📚 **12 ejercicios completamente documentados** en español
- 🎨 **Interfaz moderna** con diseño responsive
- 💡 **Comentarios educativos** explicando cada sección del código
- 🚀 **JavaScript puro** (sin TypeScript) para facilitar el aprendizaje
- 🎯 **Progresión gradual** desde conceptos básicos hasta avanzados
- 🌓 **Temas claro/oscuro** con localStorage
- 📱 **100% responsive** para todos los dispositivos
- 🐳 **Docker ready** para despliegue fácil

## 🚀 Inicio Rápido

### Instalación

```bash
# Clonar el repositorio
git clone https://github.com/USUARIO/escuela-code-lab-2026.git
cd escuela-code-lab-2026

# Instalar dependencias (requiere pnpm)
pnpm install

# Iniciar servidor de desarrollo
pnpm dev

# Construir para producción
pnpm build

# Previsualizar build de producción
pnpm preview
```

El servidor de desarrollo estará disponible en `http://localhost:4321`

### Con Docker

```bash
# Construir la imagen
docker build -t escuela-code-lab .

# Ejecutar el contenedor
docker run -p 80:80 escuela-code-lab

# Acceder en http://localhost
```

## 📚 Estructura de Contenidos

### Ejercicios Base

#### Sesión 1: Primeros Pasos con el DOM
- **Botón Mágico**: Manipulación básica del DOM y eventos
- **Mini Galería**: Sistema de galería de imágenes con lightbox
- **Modo Noche**: Toggle de tema claro/oscuro

#### Sesión 2: Componentes Interactivos
- **Slider de Imágenes**: Carrusel con navegación y auto-play
- **Menú Hamburguesa**: Navegación responsive para móviles
- **Portfolio con Filtro**: Sistema de filtrado por categorías

#### Sesión 3: Animaciones y Efectos
- **Animaciones on Scroll**: IntersectionObserver y efectos de entrada
- **Efecto Parallax**: Profundidad y movimiento con scroll
- **Contadores Animados**: Números animados y barras de progreso

#### Sesión 4: Proyecto Final
- **Portfolio Completo**: Integración de todos los conceptos aprendidos
  - Navegación responsive con menú hamburguesa
  - Slider de proyectos
  - Animaciones on scroll
  - Sistema de filtrado
  - Formulario con validación
  - Modo claro/oscuro

### Ejercicios Avanzados

- **Scroll Reveal Avanzado**: 
  - Motion One library para animaciones basadas en scroll
  - CSS Grid + Subgrid para layouts complejos
  - Keyframes y offsets personalizados
  - Curvas de Bézier y easing functions
  - Accesibilidad con prefers-reduced-motion

- **WebGL Shader Effects**: 
  - Renderizado acelerado por GPU con WebGL
  - Vertex y Fragment Shaders en GLSL
  - Simplex Noise para efectos procedurales
  - Texturas e interacción con mouse
  - TWGL.js para simplificar WebGL
  - Transformaciones 3D y perspectiva

## 🛠️ Tecnologías

- [Astro](https://astro.build) v4.16+ - Framework web estático de alto rendimiento
- HTML5 & CSS3 con variables CSS
- **JavaScript puro** (sin TypeScript) para facilitar el aprendizaje
- [Motion One](https://motion.dev) - Animaciones basadas en scroll (Web Animations API)
- [TWGL.js](https://twgljs.org) - WebGL helper library
- WebGL + GLSL para efectos gráficos avanzados
- IntersectionObserver API para scroll animations
- LocalStorage para persistencia
- Docker + Nginx para despliegue

## 📁 Estructura del Proyecto

```
/
├── src/
│   ├── layouts/
│   │   └── Layout.astro          # Layout base con estilos globales
│   ├── pages/
│   │   ├── index.astro           # Página principal con navegación
│   │   ├── base/                 # Ejercicios base (10 páginas)
│   │   │   ├── sesion1/          # DOM manipulation (3 ejercicios)
│   │   │   ├── sesion2/          # Componentes interactivos (3 ejercicios)
│   │   │   ├── sesion3/          # Animaciones y efectos (3 ejercicios)
│   │   │   └── sesion4/          # Portfolio final integrado (1 ejercicio)
│   │   └── avanzado/             # Ejercicios avanzados (2 páginas)
│   │       ├── scroll-reveal.astro   # Motion One + CSS Grid
│   │       └── webgl-shader.astro    # WebGL + GLSL shaders
│   └── styles/
│       └── global.css            # Variables CSS y reset
├── .github/
│   └── workflows/
│       └── docker-publish.yml    # CI/CD para Docker
├── public/                       # Assets estáticos
├── Dockerfile                    # Multi-stage build con Nginx
├── .dockerignore                 # Archivos excluidos del contexto Docker
├── package.json                  # Dependencias (pnpm)
├── astro.config.mjs              # Configuración de Astro
└── tsconfig.json                 # TypeScript desactivado (JavaScript puro)
```

## 🎯 Objetivos de Aprendizaje

### Fundamentos (Sesión 1-2)
1. **DOM Manipulation**: `querySelector`, `getElementById`, `createElement`, `appendChild`
2. **Eventos**: `addEventListener`, event delegation, keyboard events
3. **Arrays y Bucles**: `forEach`, `map`, `filter`, array methods
4. **Funciones**: Arrow functions, callbacks, parámetros
5. **LocalStorage**: Persistencia de datos en el navegador

### Intermedio (Sesión 3-4)
6. **Responsive Design**: Media queries, Mobile-first, flexbox/grid
7. **Animaciones CSS**: Transitions, transforms, keyframes, custom properties
8. **JavaScript APIs**: IntersectionObserver, requestAnimationFrame
9. **Validación**: Regex, validación de formularios, mensajes de error
10. **Scroll Effects**: Parallax, animaciones on scroll, sticky elements

### Avanzado
11. **Motion One Library**: Scroll-driven animations, timeline, easing functions
12. **WebGL**: Vertex/Fragment shaders, GLSL, GPU rendering
13. **Algoritmos**: Simplex Noise, interpolación lineal (lerp), transformaciones matriciales
14. **Performance**: `requestAnimationFrame`, debounce, optimización
15. **Accesibilidad**: `prefers-reduced-motion`, keyboard navigation, ARIA

## 👨‍💻 Para Estudiantes

Cada ejercicio incluye:
- ✅ **Instrucciones claras** con objetivos específicos
- ✅ **Código completamente funcional** listo para estudiar
- ✅ **Comentarios educativos en español** explicando cada línea
- ✅ **Conceptos técnicos** explicados de forma simple
- ✅ **Estilos modernos** y 100% responsive
- ✅ **Ejemplos prácticos** del mundo real
- ✅ **Progresión gradual** de dificultad

### Cómo Estudiar

1. **Lee el código** - Cada sección está numerada y comentada
2. **Ejecuta el ejercicio** - Observa cómo funciona en el navegador
3. **Modifica valores** - Experimenta cambiando parámetros
4. **Practica** - Intenta recrear el ejercicio desde cero
5. **Investiga** - Usa los comentarios como punto de partida para profundizar

### Requisitos Previos

- Conocimientos básicos de HTML y CSS
- Fundamentos de programación (variables, funciones, condicionales)
- Un navegador moderno (Chrome, Firefox, Edge, Safari)
- Editor de código (VS Code recomendado)

## � Despliegue

### GitHub Container Registry

El proyecto incluye un workflow de GitHub Actions que automáticamente:
- Construye una imagen Docker cuando se publica un tag `v*.*.*`
- Sube la imagen a GitHub Container Registry (ghcr.io)
- Mantiene solo las 5 últimas imágenes (limpia versiones antiguas)
- Limpia todas las cachés de Docker al finalizar

```bash
# Crear y publicar una nueva versión
git tag v1.0.0
git push origin v1.0.0

# La imagen estará disponible en:
# ghcr.io/USUARIO/escuela-code-lab-2026:1.0.0
```

### Ejecutar desde GHCR

```bash
docker pull ghcr.io/USUARIO/escuela-code-lab-2026:latest
docker run -p 80:80 ghcr.io/USUARIO/escuela-code-lab-2026:latest
```

## 📝 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 👥 Contribuir

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📞 Soporte

Si encuentras algún problema o tienes sugerencias:
- Abre un [Issue](https://github.com/USUARIO/escuela-code-lab-2026/issues)
- Consulta la [documentación de Astro](https://docs.astro.build)

---

**Desarrollado con 💜 para Escuela de negocios, Campus Cámara Comercio Sevilla 2026**

*Proyecto educativo para aprendizaje de JavaScript y desarrollo web frontend*
