---
title: INSTALACIÓN ORACLE WEBLOGIC SERVER
published: true
flag: false 
---

1. Nos deslogeamos como *root* y nos logeamos con el usuario que deseamos instalar, en mi caso el usario se llama *obpm*.

    ![wlg_1](../assets/obpm/centos/weblogic/wlg_1.png)

2. Abrimos una terminal y nos ubicamos en la ruta donde se encuentran los instaladores, en nuestro caso lo tenemos en */home/obpm/instaladores/3_WEBLOGIC*.

        # ls /home/obpm/instaladores/3_WEBLOGIC/

    ![wlg_2](../assets/obpm/centos/weblogic/wlg_2.png)

3. Ejecutamos el archivo **fmw_12.2.1.3.0_wls.jar**

        # java -jar fmw_12.2.1.3.0_wls.jar
    
    ![wlg_3](../assets/obpm/centos/weblogic/wlg_3.png)

4. Se muestra la siguiente ventana que da inicio de la instalación. 

    ![wlg_4](../assets/obpm/centos/weblogic/wlg_4.png)

5. Click en **Next**.    

    ![wlg_5](../assets/obpm/centos/weblogic/wlg_5.png)

6. Click en **Next**.    

    ![wlg_6](../assets/obpm/centos/weblogic/wlg_6.png)

7. En **Oracle Home** colocamos la siguiente ruta */opt/obpm/Oracle/Middleware/Oracle_Home*, click en **Next**.

    ![wlg_7](../assets/obpm/centos/weblogic/wlg_7.png)

8. Seleccionamos **WebLogic Server**, click en **Next**.  

    ![wlg_8](../assets/obpm/centos/weblogic/wlg_8.png)

9. Click en **Next**.

    ![wlg_9](../assets/obpm/centos/weblogic/wlg_9.png)

10. Click en **Install**.  

    ![wlg_10](../assets/obpm/centos/weblogic/wlg_10.png)

11. Click en **Next**.

    ![wlg_11](../assets/obpm/centos/weblogic/wlg_11.png)

12. Deseleccionar **Automatically Launch the Configuration Wizard** y click en **Finish**.

    ![wlg_12](../assets/obpm/centos/weblogic/wlg_12.png)

<div align="right">
    <a href="obpm-centos-install">
        <img src="../assets/icons/boton-back.png" title="Instalación OBPM Centos"  />
    </a>
</div>