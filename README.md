# 🏛️ Plataforma Institucional, Arquitectónica y de Telecomunicaciones (3D & 2D)

[![WebGL 3D](https://img.shields.io/badge/WebGL-3D%20Real--Time-blue?style=for-the-badge&logo=webgl)](https://threejs.org/)
[![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-v3-38bdf8?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![PowerPoint](https://img.shields.io/badge/PowerPoint-16%3A9%20Editable-d24726?style=for-the-badge&logo=microsoft-powerpoint)](distribucion_aulas_editable.pptx)
[![100% Offline](https://img.shields.io/badge/Zero--Server-100%25%20Aut%C3%B3nomo-emerald?style=for-the-badge)](index.html)

Suite integral y autónoma para el **relevamiento arquitectónico de aulas**, gestión de **turnos académicos** y diseño de la **red Wi-Fi institucional de alta densidad (AP1 a AP16)** correspondiente al **Anexo 1 Oficial: Plano de Edificio y Telecomunicaciones**.

Incluye un **Simulador 3D y Videojuego en Primera Persona (WASD)** con editor sandbox, un **Plano Interactivo 2D con 2 secciones**, una **Presentación Ejecutiva en PowerPoint (.pptx)** con formas 100% desbloqueadas y vectoriales, y planos en alta definición (`.png` y `.svg`).

---

## 📸 Vistas Previas

### 1. Simulador 3D y Videojuego Escolar (Three.js WebGL)
![Simulador 3D y Videojuego Escolar](simulador_3d_vista.png)

### 2. Plano Oficial de Redes y Telecomunicaciones (Anexo 1)
![Plano Oficial de Redes y Telecomunicaciones](plano_redes_presentacion.png)

### 3. Plano Institucional de Aulas y Turnos Multiturno
![Plano Institucional de Aulas](plano_presentacion.png)

---

## 🚀 Inicio Rápido (Uso Local en tu PC)

No se requiere instalar Node.js, `npm`, ni ejecutar servidores en segundo plano. Todo funciona al **100% con doble clic**:

1. Descarga o clona la carpeta en tu computadora.
2. Abre cualquiera de los siguientes archivos en tu navegador (Google Chrome, Microsoft Edge, Firefox):
   - **`index.html`**: Portal central con acceso a todos los módulos.
   - **`simulador_3d_interactivo.html`**: Simulador 3D y videojuego en primera persona.
   - **`plano_institucional_interactivo.html`**: Editor y visor 2D con Sección 1 (Aulas) y Sección 2 (Redes).
   - **`distribucion_aulas_editable.pptx`**: Presentación PowerPoint oficial editable.

---

## 📂 Estructura del Proyecto

```text
Plano_Aulas_Presentacion/
│
├── index.html                           # Portal central de bienvenida (ideal para GitHub Pages)
├── simulador_3d_interactivo.html        # Simulador 3D y Videojuego Sandbox (Three.js)
├── plano_institucional_interactivo.html # Plano 2D interactivo (Sección 1 Aulas + Sección 2 Redes)
├── distribucion_aulas_editable.pptx     # Presentación ejecutiva oficial 16:9 editable
│
├── simulador_3d_vista.png               # Captura en alta resolución del Simulador 3D
├── plano_redes_presentacion.png         # Plano de telecomunicaciones oficial en imagen HD
├── plano_redes_telecomunicaciones.svg   # Vector SVG nítido del tendido de red (Anexo 1)
├── plano_presentacion.png               # Plano general de aulas en imagen HD
├── plano_arquitectonico_limpio.svg      # Vector SVG arquitectónico base
│
├── lib/                                 # Librerías 3D locales para funcionamiento 100% offline
│   ├── three.min.js                     # Motor Three.js r128 minificado
│   └── OrbitControls.js                 # Control de cámara orbital Three.js
│
├── .gitignore                           # Archivos ignorados por Git
└── README.md                            # Documentación técnica completa
```

---

## 🌐 Cómo Subir este Proyecto a GitHub (Paso a Paso)

### Opción A: Mediante la Terminal / Git (Recomendado)

Si tienes **Git** instalado en tu computadora, abre **PowerShell** o la terminal dentro de esta carpeta (`Plano_Aulas_Presentacion`) y ejecuta los siguientes comandos:

```bash
# 1. Inicializar el repositorio Git local
git init

# 2. Agregar todos los archivos al seguimiento
git add .

# 3. Crear el primer commit
git commit -m "feat: proyecto institucional de aulas, redes y simulador 3D completo"

# 4. Renombrar la rama principal a 'main'
git branch -M main

# 5. Conectar con tu repositorio remoto de GitHub (reemplaza con tu URL)
git remote add origin https://github.com/TU-USUARIO/TU-REPOSITORIO.git

# 6. Subir los archivos a GitHub
git push -u origin main
```

> 💡 **Nota:** Si tu repositorio en GitHub ya contenía un archivo inicial como una licencia o README previo, puedes sincronizar antes del push con:  
> `git pull origin main --rebase` y luego `git push -u origin main`.

---

### Opción B: Subida Directa desde la Web de GitHub

1. Ingresa a [GitHub.com](https://github.com) e inicia sesión con tu cuenta.
2. Haz clic en el botón verde **"New"** para crear un nuevo repositorio:
   - Asigna un nombre (por ejemplo: `plano-institucional-3d`).
   - Elige si será **Público** o **Privado**.
   - No marques "Add a README file" (ya lo tenemos creado).
   - Haz clic en **"Create repository"**.
3. En la pantalla que aparece, haz clic en el enlace azul **"uploading an existing file"**.
4. Selecciona o arrastra todos los archivos y carpetas de `Plano_Aulas_Presentacion` a la ventana del navegador.
5. Abajo en "Commit changes", escribe un mensaje y pulsa **"Commit changes"**.

---

## 🌍 Cómo Publicar la Web Gratis en Vivo (GitHub Pages)

Puedes tener tu simulador 3D y plano 2D funcionando online en internet de forma gratuita con una URL pública para que cualquiera lo vea sin descargar nada:

1. En tu repositorio de GitHub, entra en la pestaña **Settings** (Configuración).
2. En el menú de la izquierda, haz clic en **Pages**.
3. En la sección **Build and deployment**:
   - En **Source**, selecciona `Deploy from a branch`.
   - En **Branch**, selecciona `main` y en la carpeta deja `/ (root)`.
   - Haz clic en **Save**.
4. Espera 1 o 2 minutos. GitHub generará un enlace público en la parte superior:  
   `https://TU-USUARIO.github.io/TU-REPOSITORIO/`
5. ¡Listo! Al entrar a esa URL, se abrirá el portal `index.html` con el simulador 3D y el plano interactivo funcionando directamente en internet.

---

## 🎮 Guía de Uso del Simulador 3D y Videojuego

### 1. Modos de Cámara
- **🏛️ Vista 3D Orbital (Dios / Arquitecto):**
  - **Clic Izquierdo + Arrastrar:** Rotación 360° en torno al edificio.
  - **Clic Derecho + Arrastrar:** Desplazar / Panorámica.
  - **Rueda del Ratón:** Zoom continuo hacia adentro o afuera.
  - **Botón Plano Cenital:** Conmuta a vista superior ortogonal directa (mapa 2D en 3D).
  - **Botón Centrar:** Restablece la cámara en el centro de la escuela.
- **🎮 Modo Videojuego en 1ª Persona (Walkthrough WASD):**
  - Haz clic en **"Modo Videojuego (WASD)"** arriba al centro.
  - Haz clic en cualquier parte de la pantalla para bloquear el cursor y tomar el control del avatar.
  - **`W, A, S, D`**: Caminar por pasillos y cruzar puertas hacia las aulas.
  - **`Shift`**: Correr a mayor velocidad.
  - **`Espacio`**: Salto.
  - **`F`**: Linterna de exploración nocturna.
  - **`E`**: Inspeccionar el aula o equipo que tengas enfrente.
  - **`Tab` o `Esc`**: Salir del modo videojuego y liberar el cursor.

### 2. Editor Sandbox 3D (Añadir, Modificar, Eliminar)
- **Seleccionar e Inspeccionar:** Haz clic sobre cualquier aula o nodo de red AP para abrir el panel lateral de propiedades:
  - Cambiar nombre ("Aula 24", "Laboratorio de Robótica", etc.).
  - Asignar carreras y horarios (Mañana, Tarde, Noche).
  - Modificar categoría y color visual (Tecnología, Salud, Seguridad, Gastronomía, etc.).
  - Ajustar dimensiones en metros (Ancho X, Largo Z, Alto Y) y posición en planta.
- **➕ Botón Añadir:**
  - **Nueva Aula:** Agrega un espacio lectivo 3D con muros, puerta y pupitres de alumnos.
  - **Nuevo AP Wi-Fi:** Añade un domo de techo con LED parpadeante y cúpula de cobertura.
  - **Nuevo Rack:** Crea gabinetes de telecomunicaciones de 42U.
  - **Nuevo Pasillo:** Incorpora galerías o áreas de circulación.
- **🗑️ Eliminar y Duplicar:**
  - Pulsa **"Eliminar"** en el panel lateral o presiona la tecla `Supr` (`Delete`) en tu teclado.
  - Pulsa **"Duplicar"** para clonar un aula de inmediato.
- **💾 Guardar / Cargar Proyecto:**
  - Puedes exportar tu maqueta a un archivo `.json` o importar estados previos con un solo clic.
  - Guarda automáticamente tus cambios en el almacenamiento local (`LocalStorage`) de tu navegador.
- **📸 Captura HD:**
  - Botón de cámara para descargar una foto nítida de la escena en formato PNG.

---

## 📡 Especificaciones de Telecomunicaciones (Anexo 1 Oficial)

La capa de telecomunicaciones reproduce con precisión milimétrica la infraestructura de red instalada:

### Inventario de los 16 Access Points Wi-Fi
| ID | Ubicación | IP de Gestión | Puerto / Switch Alimentador | Cobertura |
| :---: | :--- | :---: | :--- | :---: |
| **AP1** | Aula 1 (Cocina 3°) | `192.168.100.11` | Switch POE 16P (P1) | 2.4 / 5 GHz |
| **AP2** | Aula 2 (Jurídica 2°) | `192.168.100.12` | Switch POE 16P (P2) | 2.4 / 5 GHz |
| **AP3** | Aula 4 (Hig. y Seg. 1° A) | `192.168.100.13` | Switch POE 16P (P3) | 2.4 / 5 GHz |
| **AP4** | Aula 6 (Prep. Física 3°) | `192.168.100.14` | Switch POE 16P (P4) | 2.4 / 5 GHz |
| **AP5** | Aula 8 (Jurídica 3°) | `192.168.100.15` | Switch POE 16P (P5) | 2.4 / 5 GHz |
| **AP6** | Aula 9 (Hig. y Seg. 1° C) | `192.168.100.16` | Switch POE 16P (P6) | 2.4 / 5 GHz |
| **AP7** | Aula 11 (Cocina 2°) | `192.168.100.17` | Switch POE 16P (P7) | 2.4 / 5 GHz |
| **AP8** | Aula 12 (Cocina 1°) | `192.168.100.18` | Switch POE 16P (P8) | 2.4 / 5 GHz |
| **AP9** | Taller Prácticas (Informática) | `192.168.100.19` | Switch POE 16P (P9) | 2.4 / 5 GHz |
| **AP10** | Rectoría / Dirección | `192.168.100.20` | Switch P16 Rectoría (P10) | VLAN Gestión |
| **AP11** | Aula 16 (Software 1°) | `192.168.100.21` | Switch P16 Oeste (P11) | 2.4 / 5 GHz |
| **AP12** | Cocina / Depósito | `192.168.100.22` | Switch P16 Oeste (P12) | 2.4 / 5 GHz |
| **AP13** | Aula 17 (Enfermería 2°) | `192.168.100.23` | Switch P16 Oeste (P13) | 2.4 / 5 GHz |
| **AP14** | Aula 20 (Prep. Física 1°) | `192.168.100.24` | Switch POE 16P (P14) | 2.4 / 5 GHz |
| **AP15** | Pasillo Sur (Baños) | `192.168.100.25` | Switch POE 16P (P15) | Circulación |
| **AP16** | Preceptoría | `192.168.100.26` | Switch P8 Preceptoría (P16) | VLAN Gestión |

### Código de Tendido de Cableado Estructurado
- 🔴 **Línea Roja (Tendido PoE UTP Categoría 6):** Distribución de datos y energía desde el **Switch POE (P16)** en el Kiosco hacia los 16 APs a lo largo de las bandejas técnicas de los pasillos.
- 🔵 **Línea Azul (Troncal Backbone Core / ISP):** Enlace troncal gigabit que une el **Modem Fibra (ISP)** y **Router Gateway DHCP** en Rectoría, baja por el **Conector Sur** hacia el **Rack 42U** en Kiosco, y deriva a **Preceptoría** y al **Router Wi-Fi del Aula 12**.

---

## 🎨 Paleta de Especialidades Académicas

| Carrera / Área | Color Hex | Emoji | Ejemplos de Aulas |
| :--- | :---: | :---: | :--- |
| **Salud** | `#f43f5e` | 🏥 | Aula 10, Aula 17 (Enfermería) |
| **Seguridad** | `#f59e0b` | 🦺 | Aula 4, Aula 5, Aula 9, Aula 15, Aula 19, Aula 21 |
| **Tecnología** | `#6366f1` | 💻 | Aula 7, Aula 16, Taller Prácticas / Computación |
| **Sociales** | `#a855f7` | ⚖️ | Aula 2, Aula 3, Aula 8, Aula 18 (Jurídica / Periodismo) |
| **Gastronomía** | `#f97316` | 🍳 | Aula 1, Aula 11, Aula 12, Cocina Institucional |
| **Deportes** | `#22c55e` | 🏃 | Aula 6, Aula 20, Aula 23 (Preparación Física) |
| **Administración** | `#475569` | 🏛️ | Rectoría, Preceptoría, Sala de Profesores |
| **Servicios** | `#64748b` | 🔧 | Sanitarios Oeste, Sanitarios Sur, Kiosco, Depósito |
| **Libre / Disponible** | `#94a3b8` | ✨ | Aula 22, Patio Central |

---

## 🛠️ Tecnologías Utilizadas

- **Three.js (r128):** Renderizado WebGL 3D, sombras suaves PCF, materiales PBR e iluminación dinámica.
- **HTML5 Canvas 2D:** Generación procedural de texturas nítidas para letreros de aulas y minimap radar.
- **Tailwind CSS (v3):** Interfaz de usuario con paneles de vidrio translúcido (*glassmorphism*) y diseño responsivo.
- **Python `python-pptx`:** Generador automatizado de presentaciones de PowerPoint con formas vectoriales nativas desbloqueadas.
- **Vectores SVG Nativo:** Renderizado escalable para impresión en planos de gran formato sin pixelado.

---

## 📄 Licencia

Este proyecto ha sido desarrollado para uso institucional, técnico y académico. Código abierto bajo la licencia **MIT**.
