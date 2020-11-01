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

5. Seleccionamos **Create a new domain** y en **Domain Location** colocamos la ruta sugerida por el wizard */opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/domains/base_domain*, click en **Next**.

    ![domain_5](../assets/obpm/centos/domain/domain_5.png)

6. Seleccionamos **Create Domain Using Product Templates** y de la lista de templetas se suguiere seleccionar:
    + Oracle BPM Suite - 12.2.1.3.0 [soa]
    + Oracle Business Activity Monitoring - 12.2.1.3.0 [soa]
    + Oracle SOA Suite - 12.2.1.3.0 [soa]
    + Oracle Enterprise Manager Suite - 12.2.1.3.0 [em]
    + Oracle JRF - 12.2.1.3.0 [oracle_common]
    + Oracle WSM Policy Manager - 12.2.1.3.0 [oracle_common]
    + Weblogic Coherence Cluster Extension - 12.2.1.3.0 [wlserver]

    Click en **Next**.    

    ![domain_6](../assets/obpm/centos/domain/domain_6.png)

7. Click en **Next**.

    ![domain_7](../assets/obpm/centos/domain/domain_7.png)

8. En **Application location** colocamos la ruta sugerida por el wizard */opt/obpm/Oracle/Middleware/Oracle_Home/user_projects/applications/base_domain*, click en **Next**.

    ![domain_8](../assets/obpm/centos/domain/domain_8.png)

9. Llenamos los valores solicitados **Name:** *weblogic* y **Password** *welcome01*, click en **Next**.

    ![domain_9](../assets/obpm/centos/domain/domain_9.png)

10. En **Domain Mode** seleccionamos **Development** y en **JDK** seleccionamos **Oracle HostSpot 1.8.0_192**, click en Next.

    ![domain_10](../assets/obpm/centos/domain/domain_10.png)

11. Llenamos los parametros de conexión que el wizard nos solicita:

    |  NOMBRE             |  VALOR      |
    | ------------------- | ----------- |
    | **Vendor**          | Oracle      |
    | **Driver**          | Oracle's Driver (Thin) for Service connections; ... |
    | **Host Name**       | obpm.domain |
    | **DBMS/Service**    | obpmdb      |
    | **Port**            | 1521        |
    | **Schema Owner**    | DEV_STB     |
    | **Schema Password** | obpm2020  |

    Click en **Get RCU Configuration**.

    ![domain_11](../assets/obpm/centos/domain/domain_11.png)

12. Si todo esta correcto deberiamos tener una ventana similar a la siguiente, click en **Next**.

    ![domain_12](../assets/obpm/centos/domain/domain_12.png)

13. Click en **Next**. 

    ![domain_13](../assets/obpm/centos/domain/domain_13.png)

14. Si todo esta correcto deberiamos tener una ventana similar a la siguiente, click en **Next**. 

    ![domain_14](../assets/obpm/centos/domain/domain_14.png)

<div align="right">
    <a href="obpm-centos-install">
        <img src="../assets/icons/boton-back.png" title="Instalación OBPM Centos"  />
    </a>
</div>