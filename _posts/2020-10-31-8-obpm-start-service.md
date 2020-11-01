---
title: CREACIÓN DE DOMINIO
published: true
flag: false 
---

1. Nos logeamos con el usuario que hicimos la instalación, en nuestro caso el usuario es *obpm*.

        # su obpm

    ![start_1](../assets/obpm/centos/domain/start_1.png)

2. Nos dirigimos a la ruta donde instalamos el dominio, en nuestro caso es */opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/domains/base_domain*.

    ![start_2](../assets/obpm/centos/domain/start_2.png)

3. Iniciamos el servidor Weblogic, para ello ejecutamos el siguiente comando.

        # ./startWebLogic.sh

    ![start_3](../assets/obpm/centos/domain/start_3.png)

4. Si el servidor subió correctamente, deberíamos tener un mensaje en la terminal similar a la siguiente imagen.

    ![start_4](../assets/obpm/centos/domain/start_4.png)

5. Abrimos un navegador en nuestro caso usaremos Chrome y colocamos la siguiente url: **http://obpm.domain:7001/console/**.

    ![start_5](../assets/obpm/centos/domain/start_5.png)


<div align="right">
    <a href="obpm-centos-install">
        <img src="../assets/icons/boton-back.png" title="Instalación OBPM Centos"  />
    </a>
</div>