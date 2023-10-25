prueba de inyesiones sql
![image](https://github.com/Echavarriad/Doc/assets/76740912/ec9d2385-1144-4567-849b-78f7bc66f018)

atravez de los campos del formulario de login se realizaron diferentes medio de princilapmnete realizado querys sql apuntanto a diferntes tablas tenineod el conocimiento de estas

querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'

![image](https://github.com/Echavarriad/Doc/assets/76740912/4d8276e1-419c-47f6-8571-97cec374e180)
querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'

![image](https://github.com/Echavarriad/Doc/assets/76740912/a6a2c08c-9873-44a4-b477-cced4321effb)

querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'


![image](https://github.com/Echavarriad/Doc/assets/76740912/da99f522-0903-4125-a622-c1d7893ef9cc)

querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'


Utiliza el cifrado de datos en repositorios de Azure DevOps:

Azure DevOps cifra los datos almacenados en sus repositorios. Asegúrate de que tus repositorios de código, artefactos y otros recursos estén ubicados en Azure DevOps para aprovechar este cifrado.
Control de acceso y políticas de seguridad:

Configura un control de acceso adecuado para tus proyectos y repositorios. Define roles y permisos según el principio de "menos privilegios".
Implementa políticas de seguridad, como la revisión de código obligatoria y políticas de aprobación para garantizar que las implementaciones se realicen de manera segura.
Gestión de secretos y claves:

Utiliza Azure Key Vault para gestionar y proteger secretos y claves de cifrado utilizados en tus pipelines y aplicaciones.
No almacenes secretos directamente en el código o en archivos de configuración.
Seguridad en pipelines:

Utiliza las bibliotecas de variables seguras para almacenar secretos y credenciales en tus pipelines.
Evita exponer información sensible en registros o en el código de tus pipelines.
Cifrado de la comunicación:

Asegúrate de que tu comunicación con Azure DevOps esté cifrada mediante el uso de HTTPS. No transmitas datos confidenciales a través de canales no seguros.
Cumplimiento y auditoría:

Configura la auditoría y los registros de seguridad en Azure DevOps para realizar un seguimiento de las acciones y eventos relacionados con la seguridad.
Seguridad de las cuentas de usuario:

Fomenta el uso de la autenticación de múltiples factores (MFA) para proteger las cuentas de usuario.
Realiza revisiones periódicas de los accesos y permisos de usuario para garantizar que solo las personas autorizadas tengan acceso.
Capacitación y concienciación:

Proporciona formación en seguridad a tu equipo para que estén al tanto de las mejores prácticas de seguridad y cómo utilizar Azure DevOps de manera segura.
Actualizaciones y parches:

Mantén actualizados tus recursos y componentes en Azure DevOps para asegurarte de que estén protegidos contra vulnerabilidades conocidas.
Pruebas de seguridad:

Realiza pruebas de seguridad regulares en tu aplicación y en tus pipelines para identificar y remediar posibles vulnerabilidades.
Documentación y políticas de seguridad:

Documenta las políticas y procedimientos de seguridad específicos para tu organización y proyectos.
Comunica estas políticas y procedimientos a todo el equipo de desarrollo.


coapide se seguridad esclavo

Requisitos previos:

Debes tener acceso a una plataforma de virtualización (por ejemplo, VMware, Hyper-V, VirtualBox) o a un servicio en la nube (como Azure, AWS o Google Cloud) donde puedas crear y administrar VMs.
Necesitas espacio de almacenamiento adecuado para almacenar las copias de seguridad. Puedes utilizar un disco adjunto a la VM o un recurso de almacenamiento en la nube.
Pasos para configurar la VM de copias de seguridad:

Creación de la VM:

Crea una nueva VM en tu plataforma de virtualización o en la nube. Asegúrate de que la VM tenga suficientes recursos (CPU, RAM y almacenamiento) para manejar las copias de seguridad.
Sistema Operativo:

Instala un sistema operativo en la VM. El sistema operativo puede ser Windows Server, Linux u otro que sea compatible con tus necesidades y herramientas de copia de seguridad.
Conexión a la Red:

Configura la VM para que tenga acceso a la red. Puedes asignar una dirección IP estática o utilizar DHCP, según tus necesidades.
Software de Copia de Seguridad:

Instala y configura el software de copia de seguridad en la VM. Puedes usar herramientas como Veeam, Bacula, Duplicati, o incluso las herramientas de copia de seguridad integradas del sistema operativo, como Windows Server Backup.
Conexión al Servidor de Origen:

Configura la VM para que pueda conectarse al servidor que deseas respaldar. Esto puede implicar configurar credenciales de acceso y permisos de red.
Programación de Copias de Seguridad:

Configura un programa de copias de seguridad en el software instalado en la VM. Define cuándo y con qué frecuencia se deben realizar las copias de seguridad. Esto puede incluir copias de seguridad completas, incrementales o diferenciales.
Almacenamiento de Copias de Seguridad:

Configura el destino de las copias de seguridad. Puedes guardar las copias de seguridad en el disco local de la VM, un dispositivo de almacenamiento adjunto o un servicio de almacenamiento en la nube. Asegúrate de que el almacenamiento sea seguro y redundante.
Verificación de Copias de Seguridad:

Implementa procedimientos para verificar y validar las copias de seguridad. Esto puede incluir la realización de restauraciones de prueba periódicas para garantizar que las copias de seguridad sean funcionales.
Seguridad:

Asegúrate de que la VM de copia de seguridad esté protegida con medidas de seguridad adecuadas, como cortafuegos y actualizaciones regulares.
Monitoreo y Alertas:

Configura un sistema de monitoreo y alertas para supervisar el estado de las copias de seguridad y recibir notificaciones en caso de problemas.
Documentación:

Documenta todos los procedimientos y configuraciones relacionados con las copias de seguridad en la VM. Esto facilitará la gestión y la recuperación en caso de desastres.
Pruebas y Mantenimiento Continuo:

Realiza pruebas periódicas de recuperación y mantenimiento continuo de la VM y las copias de seguridad para garantizar que todo funcione según lo previsto.
