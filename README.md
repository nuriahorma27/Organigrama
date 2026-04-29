# 📊 Organigrama - Gestor Visual de Estructura Organizativa

Aplicación web interactiva para crear, editar y visualizar organigramas organizacionales de forma flexible y sin dependencias técnicas.

## ✨ Características

### Importación de Datos
- ✅ Importar desde Excel (.xlsx, .xls)
- ✅ Importar desde CSV
- ✅ Mapeo flexible de columnas
- ✅ Soporte para múltiples estructuras de datos

### Vista Organigrama
- ✅ Visualización gráfica de la estructura organizativa
- ✅ Arrastrar y soltar elementos (drag & drop)
- ✅ Edición inline de elementos
- ✅ Zoom in/out y navegación del lienzo
- ✅ Gestión de áreas, subáreas, responsables y personas
- ✅ Asignación flexible de responsables a personas
- ✅ Codificación de colores configurable

### Vista de Responsables
- ✅ Visualización jerárquica de responsables
- ✅ Agrupación de personas por responsable
- ✅ Identificación de personas sin asignar
- ✅ Reasignación rápida de responsables
- ✅ Filtrado por responsable y área

### Exportación
- ✅ Exportar a JSON (estado completo)
- ✅ Exportar a CSV (datos tabulares)
- ✅ Exportar a PNG (imagen)
- ✅ Exportar a PDF (documento)

### Persistencia
- ✅ Guardado automático en localStorage
- ✅ Importación de datos previamente exportados
- ✅ Recuperación de estado al cerrar y abrir

## 🚀 Inicio Rápido

### Opción 1: Uso local directo
1. Descarga el archivo `index.html`
2. Abre el archivo en tu navegador (no requiere servidor)
3. ¡Comienza a crear tu organigrama!

### Opción 2: Servidor local (recomendado)
```bash
# Con Python 3
python -m http.server 8000

# Con Node.js
npx http-server

# Con PHP
php -S localhost:8000
```

Luego accede a `http://localhost:8000`

## 📝 Formato de Importación

### Columnas Soportadas
El archivo debe incluir al menos una de estas columnas:

| Columna | Ejemplo | Obligatoria |
|---------|---------|-----------|
| Área | Recursos Humanos | No |
| Subárea | Selección | No |
| Responsable | Director de RR.HH. | No |
| Subresponsable | Jefe de Selección | No |
| Persona | Juan García López | No |
| Rol/Puesto | Especialista | No |
| Reporta a | Jefe de Selección | No |
| Color | #0057A8 | No |

### Ejemplo CSV
```csv
Área,Subárea,Responsable,Persona,Rol
Recursos Humanos,Selección,Director RR.HH.,Juan García,Especialista
Recursos Humanos,Selección,Director RR.HH.,María López,Asistente
Finanzas,Contabilidad,Director Finanzas,Pedro Ruiz,Contador
```

## 🎨 Identidad Visual

La aplicación utiliza la paleta de colores de **Santalucía Seguros**:

```css
--color-primary: #0057A8       /* Azul corporativo */
--color-primary-dark: #003B73  /* Azul oscuro */
--color-primary-light: #D9ECFF /* Azul claro */
--color-secondary: #4A90D9     /* Azul secundario */
--color-background: #F7FAFC    /* Fondo gris */
--color-surface: #FFFFFF       /* Blanco */
--color-border: #D6E4F0        /* Borde gris claro */
--color-text: #1F2D3D          /* Texto oscuro */
--color-muted: #6B7C93         /* Texto gris */
--color-warning: #F4B400       /* Aviso naranja */
--color-success: #34A853       /* Éxito verde */
--color-danger: #EA4335        /* Error rojo */
```

## 🎯 Casos de Uso

- **Análisis Organizacional**: Visualizar estructura jerárquica completa
- **Planificación**: Crear cambios y reorganizaciones
- **Reportes**: Exportar organigramas para documentación
- **Onboarding**: Mostrar estructura a nuevos empleados
- **Auditoría**: Verificar cadenas de mando y responsabilidades

## 📱 Compatibilidad

- ✅ Chrome/Chromium (recomendado)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Navegadores móviles (con limitaciones)

## 💾 Almacenamiento

- Datos guardados en **localStorage** del navegador
- Capacidad típica: 5-10 MB
- Persistencia: hasta que se borren datos del navegador

## 🔧 Estructura Técnica

- **HTML5**: Estructura semántica
- **CSS3**: Diseño responsive
- **Vanilla JavaScript**: Sin dependencias externas (excepto librerías CDN opcionales)
- **Canvas API**: Renderizado del organigrama
- **Drag & Drop API**: Interactividad
- **localStorage**: Persistencia de datos

### Librerías CDN Utilizadas
- `XLSX`: Lectura de archivos Excel
- `html2canvas`: Conversión a imagen
- `html2pdf`: Generación de PDF

## 📋 Requisitos Técnicos

- Navegador moderno con soporte para:
  - HTML5 Canvas
  - Drag & Drop API
  - localStorage
  - ES6 JavaScript

## 🤝 Contribuciones

Para mejoras o reportar bugs, crea un issue en el repositorio.

## 📄 Licencia

Proyecto de demostración para Santalucía Seguros.

## 📞 Contacto

Para preguntas sobre la implementación, contacta al equipo de desarrollo.

---

**Versión**: 1.0.0  
**Última actualización**: Abril 2026  
**Estado**: ✅ Producción
