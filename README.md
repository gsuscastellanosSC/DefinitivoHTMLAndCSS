# Curso Definitivo de HTML y CSS
    https://platzi.com/clases/html-css/
# 1. Web Developer Fundamentals
# Class#1
    Bienvenida al curso
# Class#2
    Frontend
        Perfiles de desarollo:
            -> Front-end(Cliente)
                * HTML
                * CSS
                    -> Frameworks de CSS
                        * Bootstrap
                        * Foundation
                        * Materialize
                    -> Preprocesadores de CSS
                        * less
                        * stylus
                        * sass
                * JS
                    -> Frameworks de JS
                        * React
                        * Angular
                        * Vue
                    -> Compiladores / Empaquetador
                        * Babel
                        * Webpack
# Class#3
    Backend
        * Diferentes lenguajes de programación
        * Diferentes frameworks
        * Infraestructura
        * Bases de datos
# Class#4
    Fullstack
# Class#5
    Páginas Estáticas vs. Dinámicas
        -> Landing pages(Páginas Estáticas)
            * Texto plano
            * No tienen un CRUD
        -> Wep Apps (Páginas Dinámicas)
            * Tienen CRUD
# 2. HTML
# Class#6
    HTML: anatomía de una página web
    <html>
        <header>
        </header>
        <body>
        </body>
        <footer>
        </footer>
    </html>
# Class#7
    Index y su estructura básica: head
# Class#8
    Index y su estructura básica: body
# Class#9
    Reto: crea tu lista de compras del supermercado
# Class#10
    Anatomía de una etiqueta de HTML
                Opening Tg
         ____________________________
        |                           |
        | Attribute     Attribute   |
        |   Name          Value     |
        |______  ___________________|
        |      ||                   |
        <a href="http://dabrook.org">Visit DaBrook</a>
        |___________________________|
                Atribute
        |_____________________________________________|
                            Element
# 3. Etiquetas multimedia
# Class#11
    Tipos de imágenes
        Lossy vs Lossless:
            * Lossless(Sin pérdida), calidad.
                -> Más pequeñas
                -> Carga más rapida
                -> Ejemplos: gif, PNG ...
            * Lossy(Con pérdida), calidad.
                -> Más grandes
                -> Carga menos rapida
                -> Ejemplos: JPG / JPEG, SVG-Vector
# Class#12
    Optimización de imágenes
        -> Tamaño recomendado: 100 KB a 70 KB <= 1 MB
# Class#13
    Etiqueta img
# Class#14
    Etiqueta figure
# Class#15
    Etiqueta video
# 4. Formularios
# Class#16
    Etiqueta form e input
# Class#17
    Calendar
# Class#18
    Autocomplete y require
# Class#19
    Select
# Class#20
    Input type submit vs. Button tag
# 5. CSS
# Class#21
    ¿Qué es CSS?
        Cascading Style Sheets
# Class#22
    ¿Cómo utilizamos CSS?: por etiqueta, selector, class y por ID
# Class#23
    Pseudo clases y pseudo elementos
# Class#24
    Anatomía de una regla de CSS
    Selector
    |  |
    |__|         Property Value
     p{          |___|
         color  : red;
        |_____|
        Property
    }
    |_________________|
        Declaration
# Class#25
    Modelo de caja
                        Top
            ________________________________
            |margin                         |
            |   ____________________________|
            |   |Border                     |
            |   |    _______________________|
    Left    |   |   |padding                | Right
            |   |   |                       |
            |   |   |   ____________________|
            |   |   |   |Content           H|
            |   |   |   |---------W---------|
            |___|___|___|___________________|
                        Bottom
                        margin-top
                         _________
                        |   12    |
                        |    |    |
            margin-left |9   .__ 3| margin-right
                        |         |
                        |____6____|
                        margin-bottom
    => El margin siempre es trasparente.
    => El background siempre es trasparente.
    => La imagen de fondo no existe.
    => El relleno es transparente.
    => Los bordes son transparentes.
    => El contenido, texto, imagnes etc.. Es visible.
# Class#26
    Herencia
# Class#27
    Especificidad en selectores
        Importancia:
            1. Hoja de estilos de agente de usuario(Estilos del navegador)
            2. Declaraciones normales en hojas de estilo de autor(style.css)
            3. Declaraciones importantes en hojas de estilos de autor(Utiliza el !important)
        Especifidad:
            Selectores                           Especifidad
                                                (+++, ++,  +,  +-,  -)  
            !important                           1,    0,   0,  0,   0  (1)
            Inline styles(enbebidos en el html)  0,    1,   0,  0,   0  (2)
            #id                                  0,    0,   1,  0,   0  (3)
            .class                               0,    0,   0,  1,   0  (4)
            tag(etiquetas html)                  0,    0,   0,  0,   1  (5)
        Reglas de cascada.
            1. Conflicto en la declaración.
            2. ¿Diferente origen o !Important?
                2.1. Si. Utiliza la declaración con el origen de mayor prioridad.
            3. No. ¿Tiene algún Inline style?
                3.1. Si. Utiliza las Inline Declaraciones.
            4. No. ¿los selectores tienen especifidad diferente?
                4.1. Si. Utiliza las declaraciones con mayor especifidad.
            5. No. Utiliza las declaraciones que vienen en su fuente original.
        Orden de las fuentes:
            En tus estilos, las declaraciones al final del documento anularán a las que sucededan antes en caso de conflicto.
# Class#28
    Demo de especificidad y orden en selectores
# Class#29
    Más sobre selectores
# Class#30
    Combinadores: Adjacent Siblings (combinators)
    Hermano Adyacente o cercano          Hermano general
    div + p{                             div ~ p{
        ...                                 ...  
    }                                    }
    Hijo                                 Desendiente
    div > p{                             div p{
        ...                                 ...
    }                                    }
# Class#31
    Combinadores: General Sibling
# Class#32            
    Combinadores: Hijo y Descendiente
# Class#33
    Medidas:
        -> Absolutas:
            NO cambia en relación a la pantalla.
                px
        -> Relativas:
            Cambiar en relación a la pantalla.
                %
                em
                rem(root em)
                max-width/max-height
                min-width/min-height
                vw(viewport width)
                vh(viewport height)
# Class#34
    Medidas  EM
        * Em(element) Tamaño de fuente del padre directo.
# Class#35    
    Medidas  REM(Recomendado para tamaños de fuentes)
        * Hereda el tamaño del elemento root.
# Class#36    
    Max/Min width 
# Links
    Combinators:
        https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Combinators
    Select the plates:
        https://flukeout.github.io/
    CSS Specificity calculator:
        https://www.codecaptain.io/tools/css-specificity-calculator
    box-sizing:    
        https://developer.mozilla.org/es/docs/Web/CSS/box-sizing
    Pseudo-classes:
        https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes
    Pseudoelementos:
        https://developer.mozilla.org/es/docs/Web/CSS/Pseudoelementos
    Why BEM:
        https://en.bem.info/methodology/faq/#why-bem
    CSS:
        https://developer.mozilla.org/es/docs/Web/CSS
    input:
        https://developer.mozilla.org/es/docs/Web/HTML/Elemento/input
    unsplash:
        https://unsplash.com/s/photos/cats
    pexels:
        https://www.pexels.com/es-es/
    verexif para quitar meta datos:
        https://www.verexif.com/
    Smart PNG and JPEG compression:
        https://tinypng.com/
    HTML elements reference:
        https://developer.mozilla.org/en-US/docs/Web/HTML/Element