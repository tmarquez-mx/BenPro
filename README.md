<div align="center">

# 📅 BenPro

### Asistente de programación académica de posgrado

*Arrastra, suelta y deja que la herramienta cuide los choques de horario por ti.*

[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=white)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-build-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-E33439?style=flat-square)](#licencia)
[![Estado](https://img.shields.io/badge/Estado-en%20uso-success?style=flat-square)](#)

[Ver demo en vivo](https://storied-elf-14cefc.netlify.app/) · [Sobre el proyecto](https://techiholic.netlify.app/colaboracion_benpro)

</div>

---

## 🎯 Qué resuelve

Programar los cursos de un posgrado cada semestre es un rompecabezas: hay que respetar las restricciones de los horarios pico, las preferencias de horario de cada docente, impedir que dos materias obligatorias de la misma generación se empalmen, y al final entregar reportes limpios para el ingreso al sistema, la aprobación de la dirección, a los profesores y al personal de apoyo.

BenPro convierte ese rompecabezas en un tablero visual de arrastrar y soltar, y se encarga de vigilar las reglas mientras la persona que coordina decide.

| Antes | Con BenPro |
|-------|-----------|
| Hojas de cálculo cruzadas a mano | Calendario visual de arrastrar y soltar |
| Choques de horario detectados tarde | Validación de empalmes en tiempo real |
| Preferencias de docentes en correos sueltos | Preferencias leídas y resaltadas en el tablero |
| Reportes rearmados uno por uno | Exportación a Word y Excel con un clic |

---

## ✨ Características principales

### 🧠 Detección de choques en tiempo real
Cada vez que se coloca una materia, la herramienta revisa tres reglas a la vez: que el mismo docente no quede empalmado, que dos obligatorias de la misma generación no coincidan, y respeta excepciones para materias equivalentes que sí pueden compartir horario (por ejemplo, métodos de maestría y doctorado que se imparten juntos).

### 🗣️ Lectura de preferencias en lenguaje natural
Las preferencias de horario se escriben como las dicta cada profesor ("Martes (14-17) / Miércoles (14-17)", "Lunes o miércoles 16-19", "Martes o miércoles por las mañanas") y BenPro las interpreta para resaltar en verde las celdas preferidas al momento de programar.

### ⚡ Autoprogramación por cohorte
Con un botón, la herramienta intenta acomodar todas las materias pendientes. Prioriza las obligatorias, agrupa por generación para concentrar los días, intenta primero el horario predeterminado, luego las preferencias del docente, y al final cualquier hueco libre sin colisión. Cada materia colocada queda etiquetada con la razón (preferencia, predeterminado o slot libre).

### 📊 Reportes listos para entregar
- Reporte por docente, con marca de horario pico y aviso de clases fuera de su preferencia, exportable a Word o copiable con formato para WhatsApp.
- Reporte consolidado por generación, en formato horizontal listo para imprimir.
- Panel de estadísticas del semestre: horas semanales y semestrales, avance de programación, distribución en horario pico y carga académica por docente.

### 🔁 Historial, deshacer y comparación de versiones
Deshacer y rehacer con Ctrl+Z y Ctrl+Y (hasta 30 pasos). Al cargar un respaldo, BenPro muestra un comparador que señala qué materias son nuevas, cuáles se eliminaron, cuáles cambiaron de horario y cuáles cambiaron de profesor, antes de aplicar nada.

### 💾 Respaldo local y en la nube
Guardado automático por ciclo en el navegador, respaldo descargable en JSON y un flujo guiado para subirlo a la carpeta compartida del equipo en OneDrive.

---

## 🛠️ Características de apoyo

- Vista para Maestría y Doctorado, con vista consolidada de ambos niveles.
- Modo claro y modo noche.
- Catálogos de docentes y materias importables y exportables (JSON, Excel o pegando directo desde una hoja de cálculo).
- Cálculo automático de la generación a partir del semestre y el periodo.
- Seminarios sin horario fijo, separados del tablero principal.
- Vista compacta de impresión y exportación a PDF.
- Manejo de errores que protege el trabajo aunque algo falle.

---

## 🧰 Tecnologías

| Capa | Herramienta |
|------|-------------|
| Interfaz | React + Vite |
| Estilos | Tailwind CSS |
| Iconos | Lucide |
| Persistencia | LocalStorage del navegador |
| Despliegue | Netlify |

---

## 🚀 Instalación local

```bash
# Clonar el repositorio
git clone https://github.com/tmarquez-mx/benpro.git
cd benpro

# Instalar dependencias
npm install

# Levantar el servidor de desarrollo
npm run dev

# Generar la versión de producción
npm run build
```

---

## 🔒 Sobre los datos

La versión real de BenPro trabaja con los catálogos oficiales del posgrado, incluyendo nombres de profesoras y profesores y sus preferencias de horario. La demo pública usa datos ficticios para ilustrar la herramienta sin exponer información de personas reales.

| | Demo pública | Versión real |
|---|---|---|
| Docentes y materias | Ficticios | Catálogo oficial del posgrado |
| Persistencia | Solo en el navegador | LocalStorage + respaldo en OneDrive |
| Reportes | Word, Excel y PDF | Word, Excel y PDF |

---

## ✒️ Autoría

Desarrollado por **Teresa Márquez** (Techiholic Labs) para la coordinación del Posgrado en Ciencias Sociales y Políticas de la Universidad Iberoamericana Ciudad de México.

🔗 [techiholic.netlify.app](https://techiholic.netlify.app/) · [GitHub @tmarquez-mx](https://github.com/tmarquez-mx)

---

## 📄 Licencia

Distribuido bajo licencia MIT. Puedes usarlo, modificarlo y adaptarlo citando la autoría original.

<div align="center">

*Hecho con cuidado para que programar un semestre deje de doler.*

</div>
