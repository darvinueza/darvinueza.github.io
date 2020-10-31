---
title: ORACLE BPM 12c INSTALLATIONS CENTOS 7
description: El presente documento pretende servir de guía para dar inicio a la instalación de un ambiente de desarrollo de Oracle Business Process Management Standard Edition en Centos 7.
published: true
---

El presente documento pretende servir de guía para dar inicio a la instalación de un ambiente de desarrollo de **Oracle Business Process Management Standard Edition** en Centos 7.

## REQUISITOS

Antes de dar inicio a la instalación, por favor **descargue** los respectivos instaladores.

+ [JDK Download](https://www.oracle.com/java/technologies/javase/javase7-archive-downloads.html)
+ [ORACLE-DB Download](https://www.oracle.com/database/technologies/oracle-database-software-downloads.html)
+ [OBPM Download](https://edelivery.oracle.com/osdc/faces/Home.jspx)

1.  Nos logueamos con el usuario *root*.

        # su

    ![1](../assets/obpm/centos/obpm/obpm_1.png)

2.  Actualizamos todos los paquetes de Centos 7.

        # yum update

    ![2](../assets/obpm/centos/obpm/obpm_2.png)

3.  Instalamos Unzip

        # yum install unzip

    ![3](../assets/obpm/centos/obpm/obpm_3.png)

4.  Cambiamos y asignamos los permisos necesarios a la carpeta **/opt**, ya que en esta ruta estarán todos los directorios y ficheros de toda la instalación.

        # chmod -R 777 /opt/
        # chown obpm /opt/

    ![4](../assets/obpm/centos/obpm/obpm_4.png)

## INSTALACIÓN

Se presenta la lista de herramientas que se requiere para completar la instalación de Oracle BPM 12c, el orden de instalación que se presenta en este manual no es algo que se deba respetar al pie de la letra, en caso de no tener previos conocimientos de la herramienta se sugiere seguir estos pasos.

1. [Instalación JDK](obpm/centos/1_JDK.md)
2. [Instalación Oracle Data Base](recursos/2_ORACLE_DATA_BASE.md)
3. [Instalación Oracle Weblogic Server](recursos/3_WEBLOGIC.md)
4. [Instalación Oracle SOA Suite](recursos/4_SOA.md)
5. [Instalación Oracle Business Process Management](recursos/5_OBPM.md)
6. [Instalación RCU](recursos/6_RCU.md)

[Link to another page](another-page).