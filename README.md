# IALegalChadwi

**IALegalChadwi** es una aplicación web desarrollada como parte de un proyecto académico en la carrera de Ingeniería en Inteligencia Artificial de la Escuela Superior de Cómputo del Instituto Politécnico Nacional (ESCOM - IPN). El sistema tiene como objetivo brindar asistencia legal automatizada mediante el uso de tecnologías modernas como React, Firebase y modelos de inteligencia artificial.

El enfoque principal del proyecto es facilitar el acceso a servicios legales, optimizar la presentación y gestión de demandas, y conectar a los usuarios con entidades jurídicas a través de un sistema inteligente, accesible y centralizado.

---

## Objetivos del Proyecto

- Facilitar la presentación de demandas legales de manera digital y asistida.
- Automatizar la asesoría legal mediante modelos de lenguaje IA.
- Proveer un sistema centralizado para el seguimiento de procesos legales.
- Permitir la conexión y gestión directa con entidades legales a través de una plataforma web.
- Servir como base para futuras integraciones con tecnologías de procesamiento de lenguaje natural y automatización legal.

---

## Características Principales

- Presentación de demandas legales a través de formularios dinámicos.
- Asesoría legal preliminar asistida por inteligencia artificial.
- Gestión y seguimiento de demandas según el tipo de usuario (demandante, demandado, legal).
- Integración con Firebase para autenticación, almacenamiento y base de datos en tiempo real.
- Arquitectura escalable para implementación futura en instituciones legales reales.

---

## Detalles
- El modelo de IA está implementado de manera local mediante una red neuronal. Se le brindó un conjunto de datos etiquetado manualmente, el cual fue utilizado para entrenar el modelo. Se definieron patrones de posibles preguntas y se proporcionaron respuestas entre las que el modelo podía elegir y enviarlas como respuesta.
- Después, estas respuestas se combinaron con el modelo de IA ollama 3.1 para crear respuesta más naturales y flexibles, con el objetivo de crear flujos de conversación más amigables para el usuario.
- Posteriormente, se conectó mediante una API el modelo de ollama 3.1 y las respuestas generadas por la IA para brindar una interfaz simple y conocida por el usuario.
- Todo lo anterior se realiza utilizando recursos locales, se utiliza una tarjeta gráfica RTX 3060 y un procesador Ryzen 7 de quinta generación.
Este aproximamiento en la implementación permitió lograr un modelo más especializado en el ámbito de las leyes, mientras que se mantenía la escalabilidad y aprovechamiento de recursos a disposición del equipo.


## Tecnologías Utilizadas

| Tecnología | Uso |
|------------|-----|
| React.js | Interfaz de usuario y SPA |
| Firebase / Firestore | Backend como servicio (BaaS), autenticación, base de datos |
| JavaScript (ES6+) | Lógica principal de aplicación |
| HTML / CSS | Estructura y estilos base del frontend |
| NLP | Procesamiento de lenguaje para asesoría legal (planeado/implementado) |

---

## Estructura del Proyecto

```
IALegalChadwi/
├── public/                 # Archivos estáticos
├── src/
│   ├── components/         # Componentes reutilizables de React
│   ├── pages/              # Vistas principales por rol (demandante, demandado, legal)
│   ├── services/           # Configuración e integración con Firebase e IA
│   └── App.js              # Componente principal de la aplicación
├── .vscode/               # Configuración del entorno de desarrollo
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```
---

## Instalación y Ejecución Local

### Requisitos

- Node.js >= 18.x
- npm >= 9.x

### Instrucciones

1. Clonar el repositorio:

```bash
git clone https://github.com/Jose2401/IALegalChadwi.git
cd IALegalChadwi
````

2. Instalar las dependencias:

```bash
npm install
```

3. Ejecutar el proyecto en modo desarrollo:

```bash
npm start
```

4. Acceder a `http://localhost:3000` desde el navegador.

---

## Roles y Funcionalidades

| Rol                 | Funcionalidades                                                     |
| ------------------- | ------------------------------------------------------------------- |
| Demandante          | Crear, consultar y dar seguimiento a demandas.                      |
| Demandado           | Acceder a demandas recibidas y responderlas.                        |
| Representante Legal | Gestionar múltiples casos, asesorar usuarios, y validar documentos. |

---

## Estado Actual del Proyecto

* [x] Estructura base del proyecto React
* [x] Configuración inicial de Firebase
* [x] Vistas por tipo de usuario
* [ ] Integración completa con IA legal (en progreso)
* [ ] Conexión con instituciones legales reales (fase de diseño)

---

## Contribuciones

Este proyecto está abierto a sugerencias, mejoras y colaboraciones. Si deseas contribuir, por favor crea un fork y envía un pull request.

---

## Créditos

**IALegalChadwi** es desarrollado como parte de un proyecto final de la materia de Ingienería de Software para Sistemas inteligentes, de la carrera de Ingeniería en Inteligencia Artificial en la **Escuela Superior de Cómputo (ESCOM)** del **Instituto Politécnico Nacional (IPN)**.

Autores principales:

* Thania P. EG
* J. Antonio CA
* José C. EM

Asesor académico: Chadwi

---

## Licencia

Este proyecto está licenciado bajo los términos de la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

