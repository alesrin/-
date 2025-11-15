# 🌳 Árbol de Conocimiento 3D - Kobalto Homeschooling

## 🌟 Descripción

**Árbol de Conocimiento 3D** es una herramienta visual e interactiva desarrollada para estudiantes de Kobalto Homeschooling. Permite a los estudiantes visualizar su progreso académico de manera inmersiva y motivadora mediante un árbol 3D que crece a medida que completan niveles en diferentes asignaturas.

### ✨ Características Principales

- **Visualización 3D Interactiva**: Árbol completamente renderizado en Three.js con controles intuitivos
- **Sistema de Ramas por Asignatura**: Cada rama representa una materia (Matemáticas, Programación, Lengua, etc.)
- **Código de Colores de Progreso**:
  - 🔴 Rojo: Requiere atención (<30%)
  - 🟡 Amarillo: En progreso (30-70%)
  - 🟢 Verde: Buen progreso (70-99%)
  - 🟨 Dorado: Excelencia alcanzada (100%)
- **Hojas y Frutos**: Las hojas representan niveles certificados, los frutos dorados niveles con excelencia
- **Gamificación**: Sistema de logros, rachas, y estadísticas motivacionales
- **Tour Guiado**: Introducción paso a paso para nuevos usuarios
- **Vistas Múltiples**: Modo 3D, 2D, vista general y detallada
- **Responsive**: Funciona en desktop, tablet y móvil

## 🚀 Demo

Abre `index.html` en un navegador moderno para ver el árbol en acción.

## 📋 Requisitos

- Navegador moderno con soporte para WebGL (Chrome, Firefox, Safari, Edge)
- No requiere instalación ni dependencias locales (usa CDNs)

## 🛠️ Instalación

```bash
# Clonar el repositorio
git clone <repository-url>

# Navegar al directorio
cd kobalto-knowledge-tree

# Abrir index.html en tu navegador
# O usar un servidor local simple:
python -m http.server 8000
# O con Node.js:
npx serve
```

## 📁 Estructura del Proyecto

```
kobalto-knowledge-tree/
├── index.html              # Archivo principal (HTML + CSS + JS integrado)
├── MEJORAS.md             # Plan completo de mejoras futuras
├── assets/                # Recursos estáticos (preparado para futuro)
│   ├── css/              # Estilos modulares (futuro)
│   ├── js/               # Scripts modulares (futuro)
│   └── img/              # Imágenes
├── docs/                  # Documentación adicional
└── README.md              # Este archivo
```

## 💡 Uso

### Navegación Básica

- **Rotar el árbol**: Click y arrastra
- **Zoom**: Rueda del ratón
- **Seleccionar rama**: Click en una rama del árbol
- **Cambiar vista**: Usa los botones superiores
- **Tour guiado**: Click en "Tour Guiado" para instrucciones

### Datos del Estudiante

Actualmente usa datos de demostración hardcodeados en `studentData`. Para usar datos reales:

1. Conecta con un backend (ver [MEJORAS.md](MEJORAS.md))
2. O modifica el objeto `studentData` en el script

## 🎨 Personalización

### Colores

Los colores principales están definidos al inicio del `<style>`:
- Verde agua: `#6efacc`
- Dorado: `#D1A517`
- Azul oscuro: `#042454`

### Asignaturas

Edita el objeto `studentData.branches` en el script para añadir/modificar asignaturas:

```javascript
{
    id: 'nueva-asignatura',
    name: 'Nueva Asignatura',
    icon: 'fa-icon-name',  // FontAwesome icon
    currentLevel: 3,
    maxLevel: 10,
    color: 0xHEXCOLOR,
    nextLevel: 'Próximo Tema',
    description: 'Descripción de la asignatura',
    lastActivity: 'Hace X días',
    predictedDays: 20
}
```

## 🔧 Tecnologías

- **Three.js** (r128): Renderizado 3D
- **Vanilla JavaScript**: Lógica de aplicación
- **CSS3**: Estilos y animaciones
- **Font Awesome 6.4.0**: Iconografía
- **Google Fonts**: Tipografías (Montserrat, Quicksand)

## 📈 Roadmap

Ver [MEJORAS.md](MEJORAS.md) para el plan completo de mejoras, incluyendo:

- Backend y persistencia de datos
- Sistema de autenticación
- IA para recomendaciones personalizadas
- Gamificación avanzada
- Modo offline (PWA)
- Integración con LMS
- Y mucho más...

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

[Especificar licencia]

## 👥 Autores

- **Equipo Kobalto Homeschooling**

## 🙏 Agradecimientos

- Three.js community
- Font Awesome
- Google Fonts

---

**Última actualización**: 2025-11-15
