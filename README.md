# 🎨 Pinceletas – Proyecto Web con Arquitectura de Microservicios



*Pinceletas* es una aplicación web desarrollada como proyecto de tesis.  

La plataforma está pensada para un emprendimiento de productos artesanales, ofreciendo a los usuarios una experiencia completa de compra online y a los administradores un panel de gestión con estadísticas y configuración del sitio.



---



## 🚀 Tecnologías principales

- *Frontend:* Angular + Bootstrap  

- *Backend:* Java (Spring Boot) – Arquitectura de microservicios  

- *Autenticación:* Firebase (Google) + JWT (Email/Password)

- *Mensajería asíncrona:* RabbitMQ 

- *Base de datos:* MySQL  

- *Testing:* JUnit + Mockito  



---



## 🛠 Microservicios y Frontend



🔗 *Frontend*  

- [pinceletas-frontend](https://github.com/agustinoliver/pinceletas-frontend)  



🔗 *Backend – Microservicios*  

- [pinceletas-user-auth-service](https://github.com/agustinoliver/pinceletas-user-auth-service)  

  - Gestión de usuarios, roles y autenticación (JWT y Firebase).  

- [pinceletas-commerce-service](https://github.com/agustinoliver/pinceletas-commerce-service)  

  - Catálogo de productos, categorías, carrito, favoritos, pedidos y estados de pedidos.  

- [pinceletas-admin-config-service](https://github.com/agustinoliver/pinceletas-admin-config-service)  

  - Configuración del sitio, dashboard de métricas y notificaciones globales.



🔗 Librerías compartidas

- [pinceletas-common-security](https://github.com/TomasHerrado/pinceletas-common-security.git)

    - Librería común para la seguridad y validación de JWT entre microservicios



🔗 Servicio auxiliar de notificaciones
- [pinceletas-notification-service](https://github.com/agustinoliver/pinceletas-notification-service.git)

  - Módulo de soporte encargado de la gestión y envío de notificaciones utilizando RabbitMQ.



---



## ✨ Funcionalidades principales



### 👤 Usuario final

- Registro, login (email/contraseña o Google) y recuperación de contraseña.  

- Exploración de catálogo con filtros y descripciones detalladas.  

- Favoritos y carrito de compras.  

- Gestión de pedidos con historial y seguimiento de estado.  

- Chatbot para consultas frecuentes y contacto directo por WhatsApp.  

- Perfil de usuario editable con datos personales.  



### 🛒 Administrador / Emprendedor

- CRUD de categorías y productos.  

- Gestión de pedidos con actualización de estados.  

- Configuración de datos de contacto, políticas y métodos de envío.  

- Dashboard con métricas y estadísticas de la plataforma.  



---



## 📊 Arquitectura



La aplicación está basada en una arquitectura de *microservicios*, desacoplando las distintas responsabilidades:  



- *User & Auth Service* → Manejo de usuarios y autenticación.

- *common security* → Librería compartida de seguridad JWT

- *Commerce Service* → Flujo comercial (productos, carrito, pedidos).  

- *Admin & Config Service* → Configuración y métricas.

- *Notification Service* → Comunicación asíncrona mediante RabbitMQ y soporte JWT entre microservicios. 

- *Frontend Angular* → Interfaz web para usuarios y administradores.  



---



## 📌 Autor

Desarrollado por *Herrado Tomas* y *Olivera Agustín*  

📍 Proyecto de Tesis – Tecnicatura en Programación
