# 🛒📚 AkibaMart 💥🥋




<img src="../../Frontend/AkibaMart/src/assets/fondo.png" alt="Fondo manga" width="700"/>
=======
<img src="./src/assets/fondo.png" width="700"/>
>>>>>>> 3029604b6e68227d0a0d449062bb4e5e3f8ceac6

**AkibaMart** es un e-commerce centrado en la venta de comics manga de distintas categorías. El proyecto cuenta con una aplicación frontend desarrollada en React y un backend completo en Node.js con Express y MongoDB. La aplicación cuenta con registro y autenticación de usuarios, manejo de productos, categorías y filtros, carrito de compra y pedidos.

---
## 📦 Tecnologías principales

### Frontend
- React 
- React Router DOM
- Axios
- CSS/SASS
- JWT para autenticación
- Ant-Design

### Backend
- Node.js
- Express
- MongoDB con Mongoose
- JWT para autenticación
- Swagger (documentación de la API)
- Dotenv, CORS
- Render 


## 🧩Funcionalidades principales

#### 🛍️ Productos

- Listado general de productos y vista de destacados en Home.
- Vista detallada con nombre, imagen, precio, descripción y categorías.
- Buscador y filtros combinables (por nombre, precio, categoría).
- Añadir productos al carrito desde el Home o desde el detalle.

#### 🛒Carrito

- Persistencia con `localStorage`.
- Vaciar carrito por completo.
- Funcionalidad de creación de pedidos.

#### 🧑 Usuarios

- Registro con validación y confirmación por email.
- Inicio de sesión con token JWT.
- Mensaje de bienvenida personalizado.
- Perfil de usuario mostrando pedidos

## 🚀 Instalación del proyecto
### Requisitos previos
- Node.js y npm instalados
- Cuenta MongoDB (Atlas o local)
- Cuenta Gmail (para servicio de email con nodemailer)

### Clonar el repositorio
```bash
git clone https://github.com/tu_usuario/akibamart.git
cd akibamart
```
### 📁 Variables de entorno

Crea un archivo .env en el backend con la siguiente información:

- PORT

- MONGO_URI=mongodb+srv://<usuario>:<password>@cluster.mongodb.net/akibamart

- JWT_SECRET=una_clave_segura

### 🔧 Instalación de dependencias
#### Backend
```
cd frontend

npm install

npm run dev
```

#### Frontend
```
cd frontend

npm install

npm run dev
```

## 📁 Estructura del proyecto
```
/frontend
  ├── src/
  │   ├── assets/
  │   ├── components/     
  │   ├── context/
  │   ├── pages/
  │   ├── services/
  │   ├── styles/     
  │   └── App.jsx
/backend
  ├── models/
  ├── routes/
  ├── controllers/
  └── server.js
  ```

## 🧠🧾 Uso de Context y Provider en la aplicación
En el proyecto AkibaMart, se utilizan Context API de React junto con Provider para manejar estados globales como la sesión del usuario o el carrito de compras. Es una forma eficaz de evitar el “prop drilling” (pasar props innecesariamente por muchos componentes).

### 🧠Context
 
El Context en React permite compartir datos globales (como el usuario o los productos) entre componentes, sin tener que pasar props manualmente en cada nivel del árbol de componentes.

1. 👤UserContext – Para login, logout y datos del usuario

El UserContext gestiona la autenticación. Proporciona el token, los datos del usuario (user) y funciones como login, logout y getUserInfo. Gracias al UserProvider, cualquier componente puede acceder a esta información usando el hook useUser().

2. 🛒📚 ProductContext – Para productos, carrito y filtros

El ProductContext maneja la lógica de productos y carrito. Expone el listado de productos (products), el contenido del carrito (cart) y funciones como getProducts, addCart y clearCart.

### 🧾Provider
El Provider es el componente que envuelve la aplicación (o parte de ella) y proporciona el valor del contexto (como el carrito o la info del usuario). Los componentes hijos pueden acceder a ese valor con useContext


El archivo App.jsx define las rutas y envuelve todo con UserProvider y ProductProvider para que los componentes hijos accedan a los datos necesarios.

## 🌐 Despliegue

### Backend 
Desplegado en: https://akibapi.onrender.com
### Frontend
Durante el desarrollo, se ejecuta localmente desde:
```
http://localhost:5173/
````
Este servidor es lanzado por Vite, un bundler moderno que permite una experiencia de desarrollo rápida y eficiente.

#### 🧪 Herramientas de inspección y depuración del Frontend:
Al ejecutar el frontend, es recomendable utilizar las herramientas de desarrollo del navegador (DevTools) para observar y depurar el comportamiento de la aplicación:

- Network:
Permite analizar las peticiones HTTP (login, carga de productos, pedidos, etc.). Es útil para verificar el estado de las respuestas, tiempos de carga y posibles errores de comunicación con la API.

- LocalStorage:
Se utiliza para guardar información persistente como el contenido del carrito. Se puede acceder a él en la pestaña "Application" (en Chrome) > "Local Storage".

- Components (React Developer Tools): 
Ayuda a inspeccionar los componentes montados, su jerarquía, props y estado. Muy útil para depurar el funcionamiento de los Context Providers y ver cómo se propagan los datos.

- Console: 
Muestra mensajes de error, logs de estado, advertencias y cualquier console.log() útil para depurar. Es recomendable vigilar esta sección para detectar problemas o flujos inesperados.

#### 📌 Buenas prácticas al ejecutar el frontend localmente
- Asegurarse de que el backend esté levantado y accesible desde el navegador.

- Verificar que no haya errores CORS (en consola o network).

- Refrescar con Ctrl + Shift + R para limpiar la caché si se observan comportamientos inesperados.

- Si se modifican archivos del contexto o rutas, reiniciar el servidor (npm run dev) para evitar estados inconsistentes.



## 👋 Despedida

Esperamos que disfrutes de la compra de tus comics manga favoritos con **AkibaMart**🥷 Cuéntanos cómo ha sido tu experiencia y si hay algo que podamos mejorar ¡Nos vemos pronto!


<<<<<<< HEAD
<img src="../../Frontend/AkibaMart/src/assets/despedida.png" alt="Fondo manga" width="700"/>
=======
<img src="./src/assets/despedida.png" alt="Fondo manga" width="700"/>
>>>>>>> 3029604b6e68227d0a0d449062bb4e5e3f8ceac6
