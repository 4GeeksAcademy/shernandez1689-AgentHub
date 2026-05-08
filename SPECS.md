# AgentHub

AgentHub es una plataforma SaaS diseñada para que las empresas accedan de forma rápida y flexible a agentes de inteligencia artificial bajo demanda. A través de AgentHub, las organizaciones pueden “alquilar” asistentes inteligentes preconfigurados, listos para integrarse en distintos procesos de negocio sin necesidad de desarrollos complejos.

Estos agentes pueden equiparse con diversas habilidades —como navegación web, lectura y análisis de documentos, gestión de calendarios o automatización de tareas— lo que permite adaptarlos a necesidades específicas en áreas como operaciones, atención al cliente, ventas o back office.
Gracias a su enfoque modular y escalable, AgentHub facilita la implementación de soluciones de IA prácticas y eficientes, reduciendo costes, aumentando la productividad y acelerando la transformación digital de las empresas.

## Especificaciones 

- Usa un html semantico 
- Tailwind via CDN

### Tareas

- Crea un index.html

### Requisitos 

El panel debe incluir las siguientes seis secciones, accesibles desde una navegación lateral persistente. Un toggle en la barra superior debe permitir cambiar toda la interfaz entre modo claro y modo oscuro usando las utilidades dark: de Tailwind.

#### Dashboard 

- ingresos totales generados (este mes)
- pérdida total por descuentos y cupones
- número de agentes activos en todos los clientes 
- número de agentes actualmente marcados como fallando 

Cada uno de estos debe ser una tarjeta de métrica visible o icono. Debajo de las tarjetas, incluye un área de marcador de posición para un gráfico de actividad semanal.

#### Gestion de usuarios

- Tabla que liste al menos 5 usuarios hardcodeados registrados (nombre, email, plan, badge de estado)
- Cada fila debe tener un dropdown de acciones — un pequeño menú activado con un botón ⋮ — con al menos dos opciones: "Ver detalle" y "Eliminar". - - Al elegir "Ver detalle" se abre un modal overlay con el registro completo del usuario. 
- El modal debe cerrarse mediante un botón y haciendo clic en el backdrop.

#### Gestion de agentes 

- Un listado de al menos 5 agentes registrados en la plataforma, mostrando nombre del agente, propietario, estado actual (activo / inactivo / fallando) y una lista de skills colapsada. Las skills asociadas a cada agente están ocultas por defecto; hacer clic en un control expandible las revela con una transición suave. Cada agente también tiene un dropdown de acciones con las opciones "Configurar" — que abre un modal con el prompt de sistema del agente — y "Eliminar".

#### Skill

Una sección dedicada al catálogo de skills disponibles al menos 4 — las capacidades que se pueden adjuntar a los agentes. Cada skill tiene un nombre, una descripción breve, y un indicador de cuántos agentes la tienen habilitada actualmente. Incluye una breve explicación dentro del panel sobre qué significa una "skill" en el contexto de AgentHub. Las skills también tienen un dropdown de acciones con "Ver detalle" y "Eliminar".

#### Contrataciones de agentes 

Una tabla que muestra todos los contratos de alquiler activos y pasados al menos 4. Cada fila debe mostrar el cliente, el agente alquilado, las skills contratadas, las fechas del contrato y el importe total pagado. Cada fila tiene un dropdown de acciones. Al elegir "Ver detalle" se abre un modal con el desglose completo del contrato, incluyendo la lista desglosada de skills contratadas y sus precios individuales.

####  Log de error

Un registro de errores (al menos 6)de ejecución de los agentes — mostrando timestamp, nombre del agente, tipo de error y una descripción breve. Los errores deben categorizarse visualmente por tipo o gravedad usando badges con código de color. Cada entrada tiene un dropdown de acciones con "Ver detalle" (abre un modal con la traza completa del error) y "Marcar como resuelto".


### Restricciones 

- Solo JS vanilla
- Sin frameworks
- Sin backend