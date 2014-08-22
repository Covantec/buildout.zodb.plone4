buildout.zodb.plone4
====================

Configuración de buildout para respaldar, restaurar y compactar Data,
ademas de otras tareas de mantenimiento para la ZODB de Plone 4.

Requerimientos
==============

Para cumplir con los requerimientos mínimos de instalación en Debian Wheezy, 
ejecute el siguiente comando: ::

  aptitude install gcc g++ make tar unzip bzip2 libssl-dev libxml2-dev zlib1g-dev libjpeg62-dev libreadline6-dev readline-common wv xpdf-utils python2.7-dev libxslt1-dev

Descargar código fuente
=======================

Para descargar el código fuente, ejecute el siguiente comando: ::

  $ git clone https://github.com/Covantec/buildout.zodb.plone4.git

Crear entorno virtual
=====================

Para la inicialización del proyecto Buildout, ejecute el siguiente comando: ::

  $ cd buildout.zodb.plone4
  $ virtualenv python2.7
  $ source ./python2.7/bin/activate

Inicialización del proyecto
===========================

Para la inicialización del proyecto Buildout, ejecute el siguiente comando: ::

  (python2.7)$ python bootstrap.py

Construcción del proyecto
=========================

Para la construcción del proyecto Buildout, ejecute el siguiente comando: ::

  (python2.7)$ ./bin/buildout

Ejecutar Zope
=============

Para iniciar la instancia Zope, ejecute el siguiente comando: ::

  (python2.7)$ ./bin/instance start

Puede acceder a la ZMI para crear su sitio Plone en la siguiente dirección http://localhost:8080/manage

Para detener la instancia Zope, ejecute el siguiente comando: ::

  ./bin/instance stop
