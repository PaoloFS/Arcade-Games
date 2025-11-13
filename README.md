# 🚀 Arcade Zone 🚀

Un sitio web de minijuegos arcade multijugador con una estética retro-neón, construido con HTML, CSS y JavaScript puro, e integrado con Firebase para autenticación y tablas de clasificación en tiempo real.

> **Nota:** Este es un proyecto de portafolio. El enlace al juego en vivo no se comparte públicamente para gestionar los costos de la cuota gratuita de la base de datos de Firebase.

---

## 🎮 Juegos Incluidos

* **⭐ Star Catcher:** Atrapa estrellas (⭐) y potenciadores (⚡, 🌟, ⏰, 🛡️) mientras esquivas bombas (💣) para conseguir la puntuación más alta en 30 segundos.
* **🧠 Memory Master:** Encuentra todos los pares de emojis (👾, 🎯, 🎲, etc.) en el menor número de movimientos posible.

## ✨ Características Principales

* **Autenticación de Google:** Los jugadores inician sesión de forma segura con sus cuentas de Google.
* **Tablas de Clasificación Globales:** Los 10 mejores puntajes para cada juego se muestran en tiempo real.
* **Puntuaciones Personales:** El sistema guarda y muestra la mejor marca personal de cada jugador.
* **Diseño Responsivo:** Se adapta perfectamente a computadoras de escritorio, tabletas y dispositivos móviles.
* **Interfaz Neón-Arcade:** Estilo visual pulido inspirado en los arcades de los 80, usando las fuentes 'Press Start 2P' y 'Orbitron'.

## 🛠️ Stack y Arquitectura

Este proyecto está construido 100% en el frontend, utilizando servicios de backend gestionados por Firebase.

* **Frontend:** HTML5, CSS3 (con Flexbox, Grid y Animaciones), JavaScript (ES6+).
* 🔐 **Autenticación:** El inicio de sesión se gestiona a través de **Firebase Authentication** con el proveedor de Google.
* 🗃️ **Base de Datos:** Las puntuaciones personales y las tablas de clasificación globales se almacenan en **Firebase Firestore**.
* 🛡️ **Seguridad (Punto Clave):** La base de datos está protegida mediante **Reglas de Seguridad de Firestore**. Esto previene que usuarios malintencionados borren o modifiquen las puntuaciones de otros.

> **Lógica de la Regla:** Las reglas están configuradas para que **cualquier usuario pueda leer** las puntuaciones (para los marcadores globales), pero **un usuario solo puede escribir o actualizar su propia puntuación** (`if request.auth.uid == userId`).

---

## 📄 Licencia

**Copyright © 2025 PaoloFS**

**Todos los derechos reservados.**

Este proyecto y su código fuente son propiedad exclusiva del autor. Queda estrictamente prohibida la reproducción, distribución, modificación o uso de este código, en su totalidad o en parte, sin el permiso previo y por escrito del autor.
