# 🖥️ Diapositivas Interactivas — Gestión de Sistemas Operativos

Una plataforma educativa interactiva en formato de presentación web para la materia de **Gestión de Sistemas Operativos**, dirigida a estudiantes de la **Licenciatura en Ingeniería en Ciberseguridad** de la Universidad Alianza Hispana.

Consolida conceptos teóricos de arquitectura del kernel con simuladores en tiempo real que se ejecutan directamente en el navegador, sin dependencias externas.

---

## 🚀 Características Principales

- ⚡ **Arquitectura Monolítica (Single-File):** Todo el contenido, estilos y lógica interactiva residen en un único archivo: `diapositivas_gestion_so.html`.
- 🎮 **4 Simuladores Interactivos:** Herramientas con JavaScript nativo para experimentar con conceptos de hardware y software.
- 🛡️ **Enfoque en Ciberseguridad:** Notas que enlazan gestión operativa con hardening, análisis forense, fugas de handles y mitigación de exploits.
- ⌨️ **Navegación Intuitiva:** Soporte para teclado (← →) y controles en pantalla adaptables a móviles.

---

## 📚 Contenido Académico Cubierto

### 1. Gestión de Memoria
- **Binding Time:** Comparativa entre asignación en Tiempo de Compilación, Carga y Ejecución (ASLR).
- **Direccionamiento:** Espacio de Direcciones Lógicas (Virtuales) vs. Físicas.
- **Estrategias de Colocación:** Fragmentación interna y externa en RAM.

### 2. Sistemas de Archivos
- **Estructura Lógica:** Directorios en árbol, hard links y symlinks.
- **Metadatos:** i-nodos, permisos, UID, GID y timestamps MAC.
- **Métodos de Acceso:** Lectura/escritura Secuencial, Indexada y por Hash.

### 3. Gestión de Procesos
- **Anatomía de Procesos:** Texto, Datos, Heap y Stack en RAM.
- **PCB:** PID/UID, descriptores de sistema (Handles).
- **Planificación:** Algoritmos Round Robin y FCFS.

### 4. Gestión de Usuarios y Seguridad
- **Autenticación Centralizada:** Active Directory (LDAP/Kerberos) y GPOs.
- **Mitigación de Vulnerabilidades:** Hardening, DAC vs MAC, DEP/NX y ASLR.

---

## 🛠️ Simuladores en Tiempo Real

| # | Simulador | Diapositiva | Descripción |
|---|-----------|-------------|-------------|
| 1 | **Traductor de Direcciones MMU** | 1 | Calcula dirección física desde lógica; dispara Segmentation Fault al sobrepasar límites. |
| 2 | **Distribuidor de Bloques RAM** | 2 | Evalúa algoritmos First Fit, Best Fit y Worst Fit con visualización de fragmentación. |
| 3 | **Algoritmo Hash y Colisiones** | 4 | Aplica $H(K) = K \bmod 7$ y muestra gestión de colisiones por encadenamiento. |
| 4 | **Ciclo de Estados de Procesos** | 6 | Simula asignación, ejecución y bloqueo de subprocesos con registros de CPU (PC, AC, SP). |

---

## 💻 Instalación y Uso

### Método Local (Recomendado)

No requiere servidores ni dependencias. Es un archivo HTML estático con Tailwind CSS via CDN.

1. Descarga `diapositivas_gestion_so.html`.
2. Haz doble clic para abrirlo en cualquier navegador moderno (Chrome, Firefox, Edge, Safari).

### Servidor de Desarrollo Rápido

```bash
python3 -m http.server 8080