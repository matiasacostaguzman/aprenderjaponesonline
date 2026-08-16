# Landing page de Matías Acosta Guzmán

Landing page estática para presentar los servicios online de enseñanza de japonés de Matías Acosta Guzmán. La propuesta combina aprendizaje estructurado, acompañamiento personalizado, experiencia de estudio en Tokio y formación en psicología aplicada al aprendizaje.

## Web en vivo

[aprenderjaponesonline.com](https://aprenderjaponesonline.com)

## Estado del proyecto

Esta documentación corresponde al contenido actual de `index.html`. La oferta, los precios y los textos comerciales pueden cambiar, por lo que el HTML debe considerarse la fuente principal antes de publicar una nueva versión.

El proyecto no utiliza framework, gestor de paquetes ni proceso de compilación: toda la estructura, los estilos y la lógica están incluidos en un único archivo HTML.

## Estructura

```text
v71/
├── index.html
├── README.md
└── images/
    ├── profile.jpg
    └── tokyo.jpg
```

- `index.html`: estructura HTML, estilos CSS y comportamiento JavaScript.
- `images/profile.jpg`: fotografía utilizada en la cabecera.
- `images/tokyo.jpg`: imagen de la sección sobre la experiencia en Japón.

## Contenido de la página

La landing está organizada en las siguientes secciones:

1. **Navegación fija**: enlaces a Inicio, Experiencia, Metodología, Planes, Preguntas Frecuentes y Solicita acceso, con menú adaptado a móvil.
2. **Presentación principal**: propuesta de valor, fotografía de Matías y resumen de los tres planes.
3. **Indicadores de experiencia**: más de 10 años de docencia, 18 meses viviendo y estudiando en Tokio, enfoque personalizado y preparación para el JLPT Nōken.
4. **Experiencia en Japón**: descripción del aprendizaje intensivo y la inmersión vivida en Tokio.
5. **Psicología y aprendizaje**: explicación del aporte de la formación psicológica a la enseñanza.
6. **Metodología**: diagnóstico inicial, progresión estructurada y acompañamiento continuo.
7. **Planes**: detalle de las tres modalidades ofrecidas.
8. **Preguntas frecuentes**: niveles, edades, modalidad, precios, soporte, progreso, preparación JLPT Nōken y redes sociales.
9. **Llamada a la acción**: consulta de plazas por WhatsApp.
10. **Pie de página**: identidad profesional, contacto y copyright.
11. **Aviso de cookies**: banner con aceptación persistida en el navegador.

## Planes mostrados

### Japonés sin ruido

- Pack grupal de 3 meses.
- Precio mostrado: ~~1500 €~~ **997 €\***.
- 4 horas semanales de formación en directo.
- Grupos reducidos de hasta 5 personas.
- Programa estructurado, materiales didácticos e infografías.
- Asesoramiento opcional sobre aspectos prácticos de la vida en Japón.
- Soporte por WhatsApp y garantía sujeta a condiciones.
- Financiación disponible.

\* Descuento sujeto a condiciones.

### Programa Intensivo de Comunicación y JLPT Nōken N5

- Pack individual de 3 meses.
- Precio mostrado: ~~6000 €~~ **3997 €**.
- 48 horas de formación individual en directo: dos sesiones semanales de 2 horas.
- Materiales, corrección opcional de ejercicios, soporte por WhatsApp y preparación del JLPT Nōken.
- Financiación disponible.

### Inmersión Total

- Plan individual de 3 meses.
- Precio mostrado: **8997 €**.
- Más de 120 horas de formación individual e intensiva en directo.
- Cinco sesiones semanales de 2 horas.
- Plan de estudio, materiales, corrección opcional, soporte prioritario y preparación del JLPT Nōken.
- Financiación disponible.

Los textos sobre alcance, condiciones, soporte y garantía reproducen la oferta comunicada en la página; no constituyen documentación contractual independiente.

## Diseño

La interfaz utiliza una estética oscura, minimalista y de posicionamiento premium.

### Paleta principal

| Uso | Color |
| --- | --- |
| Fondo principal | `#1a1a1a` |
| Fondo secundario | `#242424` |
| Tarjetas | `#2a2a2a` |
| Texto principal | `#ffffff` |
| Texto secundario | `#b0b0b0` |
| Acento dorado | `#d4af37` |
| Acento rojo | `#c41e3a` |

### Tipografías

- **Inter**: texto general e interfaz.
- **Playfair Display**: títulos.
- **Noto Serif JP**: apoyo para caracteres japoneses.

Las fuentes se cargan desde Google Fonts y los iconos desde Font Awesome 6.4.0.

## Funcionalidades

- Navegación fija que cambia de aspecto al desplazarse.
- Ocultación de la barra de navegación en móvil al bajar por la página.
- Menú móvil desplegable.
- Desplazamiento suave entre secciones.
- Animaciones de entrada mediante `IntersectionObserver`.
- Contadores animados para los indicadores de experiencia.
- Acordeón interactivo para las preguntas frecuentes.
- Compatibilidad con `prefers-reduced-motion`.
- Banner de cookies con aceptación guardada en `localStorage`.
- Enlaces directos a WhatsApp con mensaje predefinido.
- Enlaces a Instagram.
- Medición mediante Google Analytics, con el identificador `G-JCV7QC7YFV`.

## Tecnologías y servicios externos

- HTML5.
- CSS3 embebido.
- JavaScript vanilla embebido.
- Google Fonts.
- Font Awesome 6.4.0 mediante CDN.
- Google Analytics (`gtag.js`).
- WhatsApp Click to Chat.
- Instagram.

La página necesita conexión a internet para cargar las fuentes, los iconos, Analytics y los destinos externos, pero su estructura principal no requiere un servidor de aplicaciones.

## Ejecución local

Para una revisión rápida se puede abrir `index.html` directamente en el navegador. Para reproducir mejor el comportamiento de una web publicada, es preferible servir la carpeta con un servidor local, por ejemplo:

```bash
python -m http.server 8000
```

Después, abrir `http://localhost:8000`.

## Configuración que suele requerir cambios

Antes de publicar una actualización, conviene revisar en `index.html`:

- Textos, duración, precios y condiciones de cada plan.
- Importes duplicados entre el resumen superior y las tarjetas detalladas.
- Número y mensaje predefinido de WhatsApp.
- Enlaces de Instagram.
- Identificador de Google Analytics.
- Año del copyright.
- Metadatos SEO: `title` y `meta description`.
- Imágenes y textos alternativos.
- Texto y funcionamiento del aviso de cookies.

## SEO y accesibilidad incluidos

- Documento configurado en español mediante `lang="es"`.
- Etiqueta `title` y meta descripción.
- Metaetiqueta `viewport` para diseño responsive.
- Textos alternativos en las imágenes principales.
- Opción de reducir animaciones según la preferencia del sistema.

## Notas de mantenimiento

1. **Cookies y Analytics:** el aviso indica que no se utilizan cookies de terceros, pero el documento carga Google Analytics. Es necesario revisar el texto y la implementación del consentimiento conforme a la normativa aplicable antes de publicar.
2. **Contenido comercial:** las afirmaciones sobre velocidad de avance, resultados y garantía deben revisarse cuando cambien la oferta o sus condiciones.
3. **Código autocontenido:** al estar todo el CSS y JavaScript dentro de `index.html`, cualquier cambio afecta directamente a producción. Si el proyecto crece, puede ser útil separar estilos y scripts.

## Contacto

- Web: [aprenderjaponesonline.com](https://aprenderjaponesonline.com)
- Correo: [info@aprenderjaponesonline.com](mailto:info@aprenderjaponesonline.com)
- WhatsApp: [(+34) 642 34 57 11](https://wa.me/34642345711?text=Hola,%20Mat%C3%ADas,%20me%20interesan%20tus%20servicios.)
- Instagram: [@aprenderjaponesmatias](https://www.instagram.com/aprenderjaponesmatias)

## Derechos de autor

© 2026 Matías Acosta Guzmán. Todos los derechos reservados.
