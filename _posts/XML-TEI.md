---
layout: post
title: "The Text Encoding Initiative: A Basic Example Commented"
date: 2021-10-11
author: Tamar Blue
---
<?xml version="1.0" encoding="UTF-8"?>
<!-- La declaración XML indica que se trata de un documento XML, con el tipo de codificación de caracteres: por defecto es siempre UTF-8 -->

<?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/teilite.rng" 
  schematypens="http://relaxng.org/ns/structure/1.0"?>
<!-- Esta línea indica, al igual que ocurría con la declaración de tipo de documento (DTD), indica a qué modelo concreto se sujeta este documento XML. 
En el campo de TEI el esquema más utilizado es RelaxNG que tiene como extensión .rng -->

<TEI xmlns="http://www.tei-c.org/ns/1.0">
  <!-- el elemento raíz es el encargado de contener el espacio de nombre, es decir, a qué tipo de modelo pertenecer las etiquetas utilizadas.  -->
  
  <teiHeader>
    <!-- El encabezado: es una de las partes más importantes, pues contiene toda la información de metadatos, normalmente no destinados a la publicación pero
    imprescinndibles para integrar el documento en un conjunto-->
    <fileDesc>
      <titleStmt>
        <title>Título del fichero XML</title>
      </titleStmt>
      <publicationStmt>
        <p>Información sobre la publicación digital</p>
        <p>Ejemplo realizado en fecha de <date when="2019-01-29">29 de enero de 2019</date>.
        </p>
      </publicationStmt>
      <sourceDesc>
        <p>Información sobre el texto original</p>
      </sourceDesc>
    </fileDesc>
  </teiHeader>
  
  <!-- aquí empieza la parte del cuerpo de documento -->
  <text>
    <body>
      <p>El texto </p>
      <figure>
      <!--Este elemento <figure> puede eliminarse pues es solo el logo de TEI -->
        <graphic url="http://www.tei-c.org/logos/TEI-glow.png"/>
      </figure>
    </body>
  </text>
  
</TEI>
