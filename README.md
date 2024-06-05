# WinServer2016-2022
Activar Windows Server 2016 - 2022

# Primero, verificar la verión a la que podemos hacer upgrade.

Para ver la versión a la que podemos actualizarla:

Abrimos PowerShell o CMD como administrador

DISM /Online /Get-TargetEditions

# Una vez seleccionada la versión que deseamos, la establecemos.

DISM /online /Set-Edition:ServerStandard /ProductKey:XXXXX-XXXXX-XXXXX-XXXXX-XXXXX /AcceptEula

# Claves Globales no comerciales para Windows Server 2016-2022

Las siguientes claves de producto nos permitirán convertir Server 20XX Standard o Datacenter de Evaluación a completo utilizándolas con los comandos DISM, esto no activará el producto, únicamente lo convertirá en versión completa y podrá ser activado con cualquier licencia original Retail, OEM o ROK.

Windows Server 2022 Datacenter: WX4NM-KYWYW-QJJR4-XV3QB-6VM33

Windows Server 2022 Standard: VDYBN-27WPP-V4HQT-9VMD4-VMK7H

Windows Server 2019 Datacenter: WMDGN-G9PQG-XVVXX-R3X43-63DFG

Windows Server 2019 Standard: N69G4-B89J2-4G8F4-WWYCC-J464C

Windows Server 2019 Essentials: WVDHN-86M7X-466P6-VHXV7-YY726

Windows Server 2016 Datacenter: CB7KF-BWN84-R7R2Y-793K2-8XDDG

Windows Server 2016 Standard: WC2BQ-8NRM3-FDDYY-2BFGV-KHKQY

Windows Server 2016 Essentials: JCKRF-N37P4-C2D82-9YXRT-4M63B

Reinicia cuando lo solicite, para iniciar con la nueva versión.

# Instalamaos nuestra clave KMS

slmgr /ipk AquíVaTuLicencia

# Establece una dirección KMS.

slmgr /skms kms_server

# Reemplaza kms_server con un servidor válido de KMS, por ahora funciona: kms9.msguides.com, y kms8.msguides.com.

Activa Windows

slmgr /ato

Eso es todo. Ya tienes Windows Server activado permanentemente.
