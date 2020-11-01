---
title: CREACIÓN DE DOMINIO
published: true
flag: false 
---

Nos logeamos con el usuario que hicimos la instalación, en nuestro caso el usuario es *obpm*.

    # su obpm

![start_1](../assets/obpm/centos/start-service/start_1.png)

## START WEBLOGIC SERVER

+ Nos dirigimos a la ruta donde instalamos el dominio, en nuestro caso es */opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/domains/base_domain*.

        # cd /opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/domains/base_domain

    ![start_2](../assets/obpm/centos/start-service/start_2.png)

+ Ejecutamos el siguiente comando.

        # ./startWebLogic.sh

    ![start_3](../assets/obpm/centos/start-service/start_3.png)

+ Si el servidor subió correctamente, deberíamos tener un mensaje en la terminal similar a la siguiente imagen.

    ![start_4](../assets/obpm/centos/start-service/start_4.png)

+ Abrimos un navegador en nuestro caso usaremos Chrome y colocamos la siguiente url: **http://obpm.domain:7001/console/**.

    ![start_5](../assets/obpm/centos/start-service/start_5.png)

+ Nos logueamos con el usuario *weblogic*, recordar que este es el usuario administrador que configuramos al momento de instalar el dominio.

    | **usuario** | **password** |
    | ----------- | ------------ |
    | weblogic    | welcome01    |

    ![start_6](../assets/obpm/centos/start-service/start_6.png)

    ![start_7](../assets/obpm/centos/start-service/start_7.png)

+ Podemos visualizar los servidores que estan a disposición para ser usados, para ello nos dirigimos en el menú lateral y seleccionamos **Enviroemnt/Servers**. Se presentara una ventana en la que podemos visualizar información de los tres servidores [AdminServer(admin), bam_server1, soa_server1] que podemos usar como el nombre, el estado y el puerto de los mismos.

    ![start_8](../assets/obpm/centos/start-service/start_8.png)

## START BAM SERVER

+ Nos dirigimos a la ruta donde instalamos el dominio, en nuestro caso es */opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/domains/base_domain/bin/*.

        # cd /opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/domains/base_domain/bin/
    
    ![start_9](../assets/obpm/centos/start-service/start_9.png)

+ Ejecutamos el siguiente comando.

        # ./startManagedWebLogic.sh bam_server1

    ![start_10](../assets/obpm/centos/start-service/start_10.png)


+ Se nos solicitara un usuario y password administrador de weblogic, proporcionamos estos valores y esperamos que suba el servidor.

    | **usuario** | **password** |
    | ----------- | ------------ |
    | weblogic    | welcome01    |

    ![start_11](../assets/obpm/centos/start-service/start_11.png)

+ Para validar si el usuario subió correctamente podemos ir a la consola de administración de Weblogic **http://obpm.domain:7001/console/** y en **Enviroemnt/Servers** visualizar el estado del *bam_server1*.

    ![start_12](../assets/obpm/centos/start-service/start_12.png)

## START SOA SERVER

<div align="right">
    <a href="obpm-centos-install">
        <img src="../assets/icons/boton-back.png" title="Instalación OBPM Centos"  />
    </a>
</div>