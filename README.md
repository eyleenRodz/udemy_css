# CSS - Basics To Advanced for front end development (2021)

## ¿Que es CSS?

CSS (Cascading Style Sheets) es un lenguaje de diseño grafico para definir y crear la presentación de un documento estructurado escrito en un lenguaje de marcado. En el desarrollo web basicamente es lo que hace que las paginas web se vean bonitas, apoyadas claramente por una buen uso de HTML o XHTML.

### ¿Como se agrega un css a un html?

Existen 3 formas de agregar el css a un archivo html o una pagina web, en linea, por un css interno o un css externo. Tambien determina la prioridad del estilo si se agregara un estilo distinto de las 3 formas, los valores se sobrescriben dependiendo de la prioridad. En linea es mas prioritario y css externo menos prioritario. 


* en linea : Se agrega el estilo en la propiedad style de cada elemento html 
* css interno: Se agrega en la seccion head del documento la etiqueta style donde se agrega todo el css
* css externo: Se agrega en la seccion head del documento el link de donde se usaran los estilos

### ¿Como funcionan los css que no son el linea ?

Funciona con selectores que basicamente son la forma en que el css encuentra los elementos en el DOM estos se pueden realizar por varias formas 

#### Selectores

* por tipo(s. *eltname* ): Selecciona todos los elementos que coinciden con el nombre del elemento especificado
* por clase(s. *.classname* ): Selecciona todos los elementos que tienen el atributo de class especificado.
* por id (s. *#idname* ):  Selecciona un elemento basándose en el valor de su atributo id. Solo puede haber un elemento con un determinado ID dentro de un documento.
* universal (s. * ns|* * | *) : Selecciona todos los elementos. Opcionalmente, puede estar restringido a un espacio de nombre específico o a todos los espacios de nombres.
* atributo (s. [attr] [attr=value] [attr~=value] [attr|=value] [attr^=value] [attr$=value] [attr*=value] ) Selecciona elementos basándose en el valor de un determinado atributo.

#### Combinadores

* **hermanos adyacentes(s. A + B):** El combinador + selecciona hermanos adyacentes. Esto quiere decir que el segundo elemento sigue directamente al primero y ambos comparten el mismo elemento padre.
* **general de hermanos(s. A ~ B):** El combinador ~ selecciona hermanos. Esto quiere decir que el segundo elemento sigue al primero (no necesariamente de forma inmediata) y ambos comparten el mismo elemento padre.
* **hijo (s. A > B ):** El combinador > selecciona los elementos que son hijos directos del primer elemento.
* **descendientes (s. A B):** El combinador   (espacio) selecciona los elementos que son descendientes del primer elemento.
* **columna (s.  A || B):** El combinador || selecciona los elementos especificados pertenecientes a una columna.


#### Pseudoclases


Las pseudoclases permiten la selección de elementos, basada en información de estado que no está contenida en el árbol de documentos.
    Ejemplo: La regla a:visited se aplicará a todos los elementos \<a\> que hayan sido visitados por el usuario. 

#### Pseudoelementos

Los pseudoelementos son abstracciones del árbol que representan entidades más allá de los elementos HTML. Por ejemplo, HTML no tiene un elemento que describa la primera letra de un párrafo ni los marcadores de una lista. Los pseudoelementos representan estas entidades y nos permiten asignarles reglas CSS. De este modo podemos diseñar estas entidades de forma independiente.
    Ejemplo: La regla p::first-line se aplicará a la primera línea de texto de todos los elementos <p>. 
