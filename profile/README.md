# ⚡ stgo-tomLAB

> Laboratorio de desarrollo tecnológico, ingeniería de software de alto rendimiento y prototipado de hardware.

---

## 🛠️ Stack Tecnológico

- **Go (Golang)**: Microservicios, APIs de baja latencia, backend de alta concurrencia y orquestación.  
  📖 [Documentación oficial de Go](https://go.dev/doc/)
- **Rust**: Herramientas de línea de comandos (CLI) de alto rendimiento, utilidades de bajo nivel, seguridad en memoria y firmware embebido crítico.  
  📖 [Documentación oficial de Rust](https://www.rust-lang.org/learn)
- **Node.js**: Plataformas web interactivas, dashboards de control, pasarelas de pago e integraciones rápidas.  
  📖 [Documentación oficial de Node.js](https://nodejs.org/en/docs)
- **C / C++**: Programación de microcontroladores (Arduino, ESP32, AVR/ARM), firmware embebido, lectura de sensores en tiempo real y control de actuadores.  
  📖 [Documentación de C++ (cppreference)](https://en.cppreference.com/w/) | [Documentación oficial de Arduino](https://docs.arduino.cc/)
- **Docker & Contenedores**: Estandarización obligatoria de entornos de desarrollo, compilación aislada y despliegue reproducible en todos los proyectos.  
  📖 [Documentación oficial de Docker](https://docs.docker.com/)

---

## 🖥️ Infraestructura: Servidor Propio (Lab Server)

Contamos con un servidor central propio (*on-premise / bare-metal*) dedicado a soportar la operación y desarrollo continuo del laboratorio:

- **GitHub Actions Self-Hosted Runners**: Ejecución de tests y tareas de CI que requieren interacción directa con hardware físico conectado.
- **Registro Local de Contenedores y Paquetes**: Almacenamiento rápido de imágenes Docker y binarios compilados.
- **Backups y Almacenamiento Centralizado**: Respaldo seguro de telemetría, esquemáticos y configuraciones de laboratorio.
- **Hosting de Servicios Internos**: Despliegue del *Lab Bench OS*, dashboards y herramientas internas.

---

## 🚀 Herramientas Internas y Proyectos Cimiento

> [!NOTE]  
> Estas herramientas son los **cimientos internos** desarrollados *antes* de los productos finales para acelerar, estandarizar y asegurar todo el ciclo de desarrollo del equipo.

- [ ] **Secrets Manager**: Gestor y CLI liviano para cifrar y compartir variables de entorno, claves de API y credenciales del equipo sin exponerlas en repositorios. `[Go / Rust]`
- [ ] **stgo-tom CLI**: Hub unificado de línea de comandos para tareas de despliegue, diagnósticos, scaffolding y utilidades internas. `[Rust]`
- [ ] **Lab Bench OS**: Sistema de control y reserva de estaciones de trabajo, herramientas de precisión (soldadura, osciloscopios) e impresoras 3D. `[Node.js]`
- [ ] **Hardware Diagnostic & Flashing Tool**: Utilidad de banco para pruebas automatizadas de componentes electrónicos y flasheo masivo de microcontroladores. `[Rust / Go / C++]`
- [ ] **HIL (Hardware-in-the-Loop) Test Bridge**: Puente de pruebas automatizadas que valida firmware contra hardware real conectado a los runners de CI del servidor. `[Rust / C++]`
- [ ] **Lab Telemetry & Monitor Hub**: Sistema de recolección y visualización de telemetría ambiental del laboratorio y estado de los equipos. `[Go / Node.js]`
- [ ] **Docker Base DevContainers**: Plantillas Docker estandarizadas con toolchains completos preconfigurados (Go, Rust, GCC/Clang, PlatformIO, Node.js). `[Docker]`
- [ ] **Firmware OTA & Release Manager**: Servidor liviano local para versionado y distribución de actualizaciones de firmware en red local. `[Go]`

---

## 🧪 Estándares de Calidad y Flujo de Trabajo (CI/CD)

- **Docker en Todos los Proyectos**: Cada proyecto debe incluir su correspondiente `Dockerfile` y `docker-compose.yml` para garantizar que cualquier miembro del equipo pueda levantar el entorno con un solo comando.
- **GitHub Actions Obligatorio**: Ningún Pull Request (PR) será aprobado ni fusionado a las ramas principales sin antes pasar todos los checks automáticos:
  - Pruebas unitarias y de integración.
  - Linter y chequeo estricto de formato de código según el lenguaje.
  - Análisis de vulnerabilidades y seguridad en dependencias.
  - Compilación exitosa en entornos limpios basados en Docker.

---

## 📚 Enlaces Rápidos a Documentación

| Tecnología | Recurso Principal |
| :--- | :--- |
| **Go** | [Go Standard Library & Reference](https://pkg.go.dev/std) |
| **Rust** | [The Rust Programming Language Book](https://doc.rust-lang.org/book/) |
| **Node.js** | [Node.js API Documentation](https://nodejs.org/docs/latest/api/) |
| **C++** | [C++ Reference Guide](https://en.cppreference.com/w/) |
| **Arduino** | [Arduino Language Reference](https://www.arduino.cc/reference/en/) |
| **Docker** | [Docker Guides & Manuals](https://docs.docker.com/get-started/) |
