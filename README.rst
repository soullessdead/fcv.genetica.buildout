fcv.genetica.buildout
=====================

Configuraciones básicas de buildout para construir sitio de genética animal en la fcv luz

Requerimientos
==============

Para cumplir con los requerimientos mínimos de instalación en Debian Wheezy, ejecute el siguiente comando: ::

  # aptitude install gcc g++ make tar unzip bzip2 libssl-dev libxml2-dev libxslt1-dev zlib1g-dev libjpeg62-dev libreadline6-devpython2.7-dev python-pip readline-common wv xpdf-utils
  # pip install virtualenv

Descargar código fuente
=======================

Para descargar el código fuente, ejecute el siguiente comando: ::

  $ git clone https://github.com/soullessdead/fcv.genetica.buildout.git

Crear entorno virtual
=====================

Para la inicialización del proyecto Buildout, ejecute el siguiente comando: ::

  $ cd fcv.genetica.buildout
  $ virtualenv python2.7
  $ source ./python2.7/bin/activate

Inicialización del proyecto
===========================

Para la inicialización del proyecto Buildout, ejecute el siguiente comando: ::

  (python2.7)$ python bootstrap.py

Construcción del proyecto
=========================

Para la construcción del proyecto Buildout, ejecute el siguiente comando: ::

  (python2.7)$ ./bin/buildout -vvvvvvvvvN

Ejecutar Zope
=============

Para iniciar la instancia Zope, ejecute el siguiente comando: ::

  (python2.7)$ ./bin/instance fg (o start)

Puede acceder a la ZMI para crear su sitio Plone en la siguiente dirección http://localhost:8080/manage

Para detener la instancia Zope, ejecute el siguiente comando: ::

  ./bin/instance stop
