# El Atlas de las 150 Ensaladas

Una aplicación web interactiva que presenta 150 recetas de ensaladas con información detallada, incluyendo ingredientes, cantidades, instrucciones paso a paso y valores nutricionales.

## Características

- 🌱 **150 Recetas Únicas**: Colección completa de ensaladas de diferentes categorías
- 🔍 **Búsqueda y Filtros**: Busca por ingrediente o filtra por categoría
- 📊 **Visualizaciones**: Gráficos interactivos mostrando la distribución de categorías y tiempos de preparación
- 🌙 **Modo Oscuro**: Toggle para cambiar entre modo claro y oscuro
- 📱 **Responsive**: Diseño adaptativo para todos los dispositivos
- 📋 **Información Detallada**: Cada receta incluye:
  - Cantidades precisas de ingredientes
  - Instrucciones paso a paso
  - Valores nutricionales (calorías, proteínas, carbohidratos, grasas, fibra)
  - Tiempo de preparación
  - Número de porciones

## Tecnologías Utilizadas

- HTML5
- Tailwind CSS (via CDN)
- Chart.js para visualizaciones
- Font Awesome para iconos
- JavaScript vanilla

## Despliegue en Vercel

### Opción 1: Desde la Interfaz Web de Vercel

1. **Preparar el repositorio Git** (si aún no lo tienes):
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. **Subir a GitHub**:
   - Crea un nuevo repositorio en GitHub
   - Conecta tu repositorio local y haz push:
     ```bash
     git remote add origin https://github.com/tu-usuario/atlas-ensaladas.git
     git branch -M main
     git push -u origin main
     ```

3. **Desplegar en Vercel**:
   - Ve a [vercel.com](https://vercel.com)
   - Inicia sesión con tu cuenta de GitHub
   - Haz clic en "Add New Project"
   - Importa tu repositorio de GitHub
   - Vercel detectará automáticamente la configuración
   - Haz clic en "Deploy"

### Opción 2: Usando Vercel CLI

1. **Instalar Vercel CLI**:
   ```bash
   npm i -g vercel
   ```

2. **Desplegar**:
   ```bash
   vercel
   ```
   
   Sigue las instrucciones en la terminal para:
   - Iniciar sesión en Vercel
   - Configurar el proyecto
   - Confirmar el despliegue

3. **Para producción**:
   ```bash
   vercel --prod
   ```

### Opción 3: Arrastrar y Soltar (Drag & Drop)

1. Ve a [vercel.com/new](https://vercel.com/new)
2. Arrastra la carpeta del proyecto directamente a la página
3. Vercel desplegará automáticamente tu sitio

## Estructura del Proyecto

```
atlas_ensalada/
├── index.html          # Archivo principal (Vercel lo servirá automáticamente)
├── home.html          # Archivo original (puedes eliminarlo después)
├── package.json       # Configuración del proyecto
├── vercel.json        # Configuración de Vercel
└── README.md          # Este archivo
```

## Notas

- El archivo `index.html` es el punto de entrada principal
- Vercel servirá automáticamente el archivo `index.html` en la raíz
- No se requiere build process ya que es un sitio estático
- Todas las dependencias se cargan desde CDN

## Personalización

Puedes modificar:
- Los colores en la configuración de Tailwind dentro de `index.html`
- Las recetas en el array `coreRecipes` en el JavaScript
- Los estilos en la sección `<style>` del HTML

## Licencia

MIT
