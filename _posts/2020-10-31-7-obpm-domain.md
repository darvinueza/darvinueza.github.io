---
title: CREACIÓN DE DOMINIO
published: true
flag: false 
---

1. Nos deslogeamos como *root* y nos logeamos con el usuario que deseamos instalar, en mi caso el usuario se llama *obpm*.

        # su obpm

    ![domain_1](../assets/obpm/centos/domain/domain_1.png)

2. Abrimos una Terminal y vamos a la ruta: **/opt/obpm/Oracle/Middleware/Oracle_Home/oracle_common/common/bin**

    ![domain_2](../assets/obpm/centos/domain/domain_2.png)

3. Ejecutamos el archivo **config.sh**.

    ![domain_3](../assets/obpm/centos/domain/domain_3.png)

4. Se abre el Asistente de Configuración del Dominio.

    ![domain_4](../assets/obpm/centos/domain/domain_4.png)

5. Seleccionamos **Create a new domain** y en **Domain Location** colocamos la ruta sugerida por el wizard */opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/domains/base_domain* , click en **Next**.

    ![domain_5](../assets/obpm/centos/domain/domain_5.png)

6. Seleccionamos **Create Domain Using Product Templates** y de la lista de templetas se suguiere seleccionar:
    + Oracle BPM Suite - 12.2.1.3.0 [soa]
    + Oracle Business Activity Monitoring - 12.2.1.3.0 [soa]
    + Oracle SOA Suite - 12.2.1.3.0 [soa]
    + Oracle Enterprise Manager Suite - 12.2.1.3.0 [em]
    + Oracle JRF - 12.2.1.3.0 [oracle_common]
    + Oracle WSM Policy Manager - 12.2.1.3.0 [oracle_common]
    + Weblogic Coherence Cluster Extension - 12.2.1.3.0 [wlserver]

    click en **Next**.    

    ![domain_6](../assets/obpm/centos/domain/domain_6.png)

7. Click en **Next**.

    ![domain_7](../assets/obpm/centos/domain/domain_7.png)

<div align="right">
    <a href="obpm-centos-install">
        <img src="../assets/icons/boton-back.png" title="Instalación OBPM Centos"  />
    </a>
</div>