# ¿Qué es un lenguaje de marcas?
Una marca es una señal que delimita un fragmento de texto para realizar algún procesamiento sobre ese texto. 
## Caracteristicas generales de los lenguajes de marcas ##
- Está compuesto por únicamente texto.
- Las etiquetas se mezclan con el contenido.
- El mismo documento puede ser interpretado de diferentes formas.
- Se inventó para visualizar documentos de texto.
- Se puede combinar un mismo archivo con otros lenguajes.
## Clasifica los lenguajes de marcas e identifica los más relevantes ##
1. De presentación:
   Indica el formato del texto, sin especificar su estructura. Ej: RTF, TeX

2. Descriptivo:
   Indica las diferentes partes en las que se estructura el documento, sin especificar cómo deben representarse. Ej: XFML,OWL

3. Híbrido:
   Lenguajes que contienen marcas de los dos tipos anteriores indistintamente. Ej: WML, XHTML.
## Indica los distintos ámbitos de aplicación de los lenguajes de marcas ##
Desarrollo web -->  El uso más extendido de documentos electrónicos es en forma de páginas web.

Ámbito científico --> En entornos científicos es muy común el uso de fórmulas
matemáticas complejas.

Gráficos vectoriales --> Los formatos de imágen más habituales son jpg, png y gif.Todos ellos son mapas de bits que tienen el inconveniente de que cuando su tamaño crece pierden definición

Metainformación --> Un metacontenido no es más que la información relativa al contenido del documento

Base de datos --> Al estar la información altamente estructurada se puede crear una base de datos mediante un LM, la cual permitiría un acceso a la información extremadamente rápido 

Intercambio de información --> Compartir grandes volúmenes de información entre plataformas de software y sistemas operativos diferentes de forma sencilla, segura y, sobre todo, fiable

Mensajería -->  Respecto al intercambio de mensajes se busca la flexibilidad y sencillez que ofrece un LM para intercambiar documentos electrónicos a través de mensajes de correo electrónico

## Inserta un trozo de código de cada uno de los lenguajes de marcas que se indican a continuación. Añadir a cada trozo de código un pequeño resumen sobre su estructura y la aplicación asociada que los procesa ##
1. HTML:
   <h1>
   <p>
   Hola Mundo
   </p>
   </h1>
   Estructura: HTML utiliza etiquetas que van entre < > para definir la estructura de páginas web. Las etiquetas son < html >, < head >, < body >, < h1 > y < p > Aplicación: Navegadores web, procesan HTML para mostrar páginas web.
2. iCalendar:   
    BEGIN:VCALENDAR
    VERSION:2.0
    PRODID:-//Ejemplo Corp//Calendario de Ejemplo//EN
    BEGIN:VEVENT
    UID:1234567890
    DTSTAMP:20231002T120000Z
    DTSTART:20231002T130000Z
    DTEND:20231002T140000Z
    SUMMARY:Reunión de trabajo
    DESCRIPTION:Revisión del proyecto X
    LOCATION:Oficina
    END:VEVENT
    END:VCALENDAR
    Estructura: iCalendar utiliza bloques de propiedades dentro de BEGIN y END, como VEVENT para definir eventos, junto con campos como DTSTART y SUMMARY
    Aplicación: Usado en calendarios como Google Calendar, Microsoft Outlook o Apple Calendar.
3. vCard:
    BEGIN:VCARD
    VERSION:3.0
    FN:Juan Pérez
    ORG:Empresa Ejemplo S.A.
    TEL;TYPE=WORK,VOICE:(555) 123-4567
    EMAIL:juan.perez@ejemplo.com
    END:VCARD
    Estructura: vCard define tarjetas de contacto electrónicas con atributos como FN, ORG y TEL.
    Aplicación: Utilizado en aplicaciones de contactos como Google Contacts, Apple Contacts o Microsoft Outlook
4. KML
   <?xml version="1.0" encoding="UTF-8"?>
    <kml xmlns="http://www.opengis.net/kml/2.2">
    <Placemark>
        <name>Ubicación de Ejemplo</name>
        <description>Este es un marcador de ejemplo.</description>
        <Point>
        <coordinates>-122.0822035425683,37.42228990140251,0</coordinates>
        </Point>
    </Placemark>
    </kml>
    Estructura: KML se utiliza para representar datos geográficos
    Aplicación: Procesado por Google Earth, Google Maps, y otras herramientas de mapeo geográfico
5. RSS:
    <?xml version="1.0"?>
    <rss version="2.0">
    <channel>
        <title>Noticias de Ejemplo</title>
        <link>http://www.ejemplo.com</link>
        <description>Últimas noticias del sitio de ejemplo</description>
        <item>
        <title>Título de la noticia 1</title>
        <link>http://www.ejemplo.com/noticia1</link>
        <description>Descripción de la noticia 1</description>
        <pubDate>Mon, 02 Oct 2023 12:00:00 GMT</pubDate>
        </item>
    </channel>
    </rss>
    Estructura: Un archivo RSS utiliza etiquetas como < channel> para definir el canal y < item> para los elementos de noticias.
    Aplicación: Procesado por lectores RSS como Feedly, Inoreader, y otros agregadores de noticias.
