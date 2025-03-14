# Renombrador de PDFs Académicos

Una extensión para Chrome y Firefox que renombra automáticamente los PDFs descargados desde sitios académicos, utilizando metadatos como autor, título, año y revista.

## Descripción

Este complemento intercepta las descargas de archivos PDF desde sitios web académicos (journals, repositorios, bases de datos) y los renombra automáticamente utilizando un formato predefinido basado en los metadatos extraídos de la página. Esto te ayuda a mantener tus artículos académicos organizados con nombres descriptivos y consistentes.

El formato predeterminado de renombrado es:
```
PrimerAutor_TítuloRecortado_Año_Editorial.pdf
```

Por ejemplo, un artículo con título "Developing composite indicators for agricultural sustainability assessment" de Talukder y Hipel publicado en Resources en 2020, se renombrará como:
```
Talukder_Developing-composite-indicators_2020_Resources.pdf
```

## Características

- 📌 Renombrado automático de PDFs académicos
- 🔍 Extracción inteligente de metadatos (autor, título, año, revista)
- ⚙️ Formato personalizable para el nombre de archivo
- 🔔 Notificaciones de archivos renombrados
- 🧩 Compatible con múltiples navegadores (Chrome, Firefox, Edge)

## Instalación

### Chrome
1. Descarga el código o clona este repositorio
2. Abre `chrome://extensions/` en tu navegador
3. Activa el "Modo desarrollador" (esquina superior derecha)
4. Haz clic en "Cargar descomprimida" y selecciona la carpeta del proyecto

### Firefox
1. Descarga el código o clona este repositorio
2. Abre `about:debugging#/runtime/this-firefox` en tu navegador
3. Haz clic en "Cargar complemento temporal..."
4. Selecciona el archivo `manifest.json` en la carpeta del proyecto

## Uso

1. Navega a cualquier sitio académico (journal, repositorio, etc.)
2. Descarga un PDF normalmente
3. La extensión interceptará la descarga y renombrará el archivo automáticamente
4. Puedes personalizar el formato de renombrado en la página de opciones de la extensión

## Personalización

Puedes personalizar el comportamiento de la extensión accediendo a sus opciones:

1. Haz clic en el ícono de la extensión en la barra de herramientas
2. Selecciona "Opciones"
3. Configura el formato de nombrado utilizando las siguientes palabras clave:
   - `author`: Apellido del primer autor
   - `title`: Versión abreviada del título
   - `year`: Año de publicación
   - `journal`: Nombre de la revista o editorial

## Compatibilidad

Esta extensión es compatible con:
- Google Chrome (versión 88 o superior)
- Mozilla Firefox (versión 86 o superior)
- Microsoft Edge (basado en Chromium, versión 88 o superior)

## Limitaciones

- La calidad del renombrado depende de los metadatos disponibles en la página web
- Algunos sitios pueden no proporcionar metadatos estandarizados
- En caso de metadatos faltantes, se utilizan valores predeterminados

## Solución de problemas

Si la extensión no está renombrando los PDFs:
1. Verifica que esté habilitada en el administrador de extensiones
2. Asegúrate de que estás descargando desde un sitio académico con metadatos
3. Comprueba que el archivo sea realmente un PDF
4. Revisa la consola de desarrollador para ver si hay errores

## Contribuir

Las contribuciones son bienvenidas. Si deseas mejorar esta extensión:
1. Haz un fork del repositorio
2. Crea una rama para tu característica (`git checkout -b feature/amazing-feature`)
3. Haz commit de tus cambios (`git commit -m 'Add some amazing feature'`)
4. Push a la rama (`git push origin feature/amazing-feature`)
5. Abre un Pull Request

## Autor
[Elimelec Munoz](https://github.com/elimelec-zz)  
Sitio web: [krafficdesign.com](https://www.krafficdesign.com/)

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.
