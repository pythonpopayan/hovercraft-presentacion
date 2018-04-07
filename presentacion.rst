:title: Hackea tus presentaciones con Hovercraft
:author: Pedro Rivera
:description: hacer presentaciones tipo prezi con texto restructurado
:keywords: presentation, restructuredtext, impress.js, tutorial, python
:css: pythonista.css

.. footer::

   Python Cali - 2018


----

=============

Pedro Rivera

----

cuando hago una presentacion...
==================================

- quiero concentrarme en el contenido
- quiero que sea portable
- si sabe a python.... mejor!

----

y se hizo Hovercraft
=======================

- usar texto restructurado para definir contenido y comportamiento
- usar css para la parte visual
- usar impress.js para hacer todo web


----

como empezar con Hovercraft
=============================

- instalas hovercraft
- creas el archivo de tu presentacion
- creas los estilos de tu presentacion
- compilas tu proyecto

----

instalar
===========

instalas Hovercraft con pip (en mi caso, para xubuntu, con pip3)

.. code-block:: bash

    sudo pip3 install hovercraft

----

archivo de presentacion (rst)
===============================

archivo en texto restructurado, puede lucir asi:

.. code-block:: restructuredtext

    # un comentario ;)
    # los meta-datos
    :title: Hackea tus presentaciones con Hovercraft
    :author: Pedro Rivera
    :description: hacer presentaciones tipo prezi con texto restructurado
    :keywords: presentation, restructuredtext, impress.js, tutorial, python
    :css: pythonista.css
    # inicio de primera diapositiva

    ----

    mi primera diapositiva

    ----


----

estilos de presentacion
=========================

se usa css para definir como se van a ver las cosas

.. code-block:: css

    h1, h2, h3, h4 {
        font-weight: normal;
        margin-bottom: 0.1em;
        margin-top: 0.1em;
        color: purple;
    }

css comun y corriente...
si esta feo, no me juzguen, soy programador ;)

----

:data-y: 1000
:data-x: r0
:data-rotate-y: 90

pimp my slides: transiciones
==============================

podemos definir translaciones y rotaciones en 3d con directivas,
las que acaban de ver se crearon con las siguientes:

.. code-block:: restructuredtext

    :data-y: 1000
    :data-x: r0
    :data-rotate-y: 90


----

:data-y: -1000
:data-scale: 5

pimp my slides: zoom
==============================

de igual manera podemos definir acercamientos

.. code-block:: restructuredtext

    :data-y: -1000
    :data-scale: 5


----

:data-scale: 1
:data-y: 3000

compilar la presentacion
==========================

significa sacar una carpeta con una pagina web estatica

.. code-block:: bash

    hovercraft mi_presentacion.rst carpeta_de_destino

----

:data-y: 4000

mi hoja de vida en hovercraft

----

:data-y: 5000

las kriptonitas de hovercraft
===============================

- 3D rendering (te estoy mirando, Firefox ¬¬)
- moviles

----

:data-y: 6000

GRACIAS

.. image:: Fajardo.png
