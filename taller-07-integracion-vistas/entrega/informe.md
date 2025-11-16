# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 7 - Integración de Vistas de Arquitectura_

## 👥 Integrantes del equipo
- Juan David Cetina Gómez (juancego@unisabana.edu.co)
- Ana Lucía Quintero Vargas (anaquiva@unisabana.edu.co)
- Mariana Salas Gutiérrez (marianasalgu@unisabana.edu.co)

## 🧠 Descripción general del trabajo

El objetivo de este taller fue integrar todas las vistas arquitectónicas que han sido desarrolladas en torno a los temas de negocio, información, aplicaciones, infraestructura y seguridad, pudiéndose evidenciar en un único artefacto coherente que permitiera visualizar cómo se relacionan y cómo soportan los objetivos estratégicos del cliente.

Para el caso de Zajana S.A.S., se decidió consolidar el trabajo previo en una wiki estructurada (link indicado en tablero-integrado-cliente.md). Esta wiki actúa como un repositorio central donde se organiza, conecta y explica toda la arquitectura diseñada durante las semanas anteriores. Esto da como resultado un tablero integrado que combina textos explicativos, decisiones clave y la mayoría de los diagramas formales desarrollados, permitiendo una comprensión unificada de la arquitectura empresarial del cliente.

## 🔧 Proceso de desarrollo
Para la construcción del Wiki se siguió un proceso incremental basado en la recopilación, organización y posterior alineación de todas las vistas ya elaboradas previamente. Primero se revisaron los entregables donde se habían modelado las vistas de negocio, información, aplicaciones, infraestructura y seguridad con sus respectivos diagramas (BPMN, modelos ER, diagramas C4, infraestructura lógica y STRIDE). A partir de ello, se tomó la decisión de poder integrar, limpiar y relacionar lo que ya estaba construido.

En cada vista se añadieron tres elementos principales: el objetivo de la vista, una descripción del estado actual y futuro (sugerencias realizadas), junto con una breve relación que se establecen con las demás capas. Adicionalmentem se puede incluir que las herramientas mayormente empleadas incluyeron el otro repositorio de la wiki Draw.io para los diagramas del curso.

## 🧩 Análisis del modelo propuesto
Incluya un análisis sobre:

- **Cómo se estructura el modelo entregado**

El modelo se estructura en torno a cinco vistas principales (Negocio, Información, Aplicaciones, Infraestructura y Seguridad), cada una con su propio objetivo, descripción y conjunto de diagramas. Estas vistas se organizan en la wiki siguiendo una secuencia lógica: se parte de los procesos de negocio y las capacidades organizacionales, luego se describen los datos que soportan dichos procesos, después se presentan las aplicaciones que los implementan, posteriormente se detalla la infraestructura tecnológica que los habilita y, finalmente, se incorporan los controles de seguridad que envuelven a todas las capas. Cada vista reutiliza conceptos de las anteriores (por ejemplo, procesos que usan entidades de datos o aplicaciones que consumen esos datos), lo que permite mantener trazabilidad entre decisiones de diseño y elementos arquitectónicos.

- **Cómo representa las necesidades del cliente**

El modelo representa las necesidades del cliente al centrarse explícitamente en el producto Macia y en la generación de *scores* analíticos para la evaluación de riesgo crediticio. La vista de negocio recoge procesos como la identificación de oportunidades, el diseño de soluciones y la gestión de fuentes de información, alineados con la necesidad de tomar decisiones de crédito más precisas. La vista de información refleja las entidades y datos que el cliente realmente utiliza (clientes, transacciones, cartera, empleadores, indicadores de riesgo), mientras que la vista de aplicaciones muestra cómo APIs, portales y sistemas externos colaboran para entregar esos *scores* a bancos, *fintech* y demás usuarios. Las vistas de infraestructura y seguridad, por su parte, responden a requerimientos de disponibilidad, escalabilidad y cumplimiento normativo propios del sector financiero, utilizando servicios de Azure y, en la versión futura, Snowflake como plataforma analítica central.

- **Qué supuestos se tomaron**

Entre los principales supuestos se encuentran: 
  * Zajana S.A.S. cuenta con la madurez tecnológica y organizacional para operar sobre Azure y Snowflake.
  * Las fuentes de información externas pueden integrarse mediante APIs y mecanismos de intercambio de datos relativamente estables.
  * Los clientes del producto Macia requieren niveles altos de disponibilidad, trazabilidad y seguridad por estar regulados por la Superintendencia Financiera.

## 📈 Diagrama final entregado

A continuación, se presenta el link a la wiki con la integración de las vistas arquitectónicas:

[https://github.com/MariSalas23/AREM-Wiki/wiki/Integraci%C3%B3n-de-Vistas-%E2%80%90-Zajana-S.A.S.](https://github.com/MariSalas23/AREM-Wiki/wiki/Integraci%C3%B3n-de-Vistas-%E2%80%90-Zajana-S.A.S.)

## 📋 Tabla

La siguiente tabla resume cada vista, sus principales diagramas y la relación que guarda con las demás:

| Vista                | Resumen breve                                                                                                        | Diagramas principales                                         | Relación con otras vistas                                                                                                    |
|----------------------|----------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|
| Negocio              | Describe los procesos clave de Zajana y cómo se gestiona el ciclo de vida del producto Macia y la migración a Snowflake. | BPMN de procesos clave, BPMN de migración                     | Define qué actividades requieren datos (Información), qué funciones deben soportar las aplicaciones y qué capacidades debe habilitar la infraestructura. |
| Información          | Modela las entidades de datos, sus atributos y relaciones que soportan el cálculo de *scores* y la operación de Macia. | Modelo Entidad–Relación (ERD)                                 | Provee los objetos de información que consumen los procesos de negocio, las APIs de Aplicaciones y los servicios de Infraestructura y Seguridad.          |
| Aplicaciones         | Muestra los sistemas y contenedores que implementan la lógica de negocio y exponen servicios a clientes y operadores. | C1 (Contexto), C2 (Contenedores actual), C2 mejora (Snowflake) | Conecta procesos de Negocio con Datos específicos (Información) y se apoya en la Infraestructura para desplegar portales, APIs y servicios analíticos.   |
| Infraestructura      | Detalla los servicios de Azure y su posterior evolución hacia Snowflake, incluyendo redes, cómputo, almacenamiento y analítica. | Diagramas de infraestructura actual y mejorada                | Es la base técnica sobre la que se despliegan las Aplicaciones, aloja los repositorios de Información y sirve de ancla para los controles de Seguridad.   |
| Seguridad            | Recoge los controles de identidad, protección de datos, monitoreo y cumplimiento normativo aplicados a toda la solución. | Tabla STRIDE, checklist normativo Ley 1266/1581, ISO 27001    | Envuelve al resto de vistas garantizando que procesos, datos, aplicaciones e infraestructura cumplan requisitos de confidencialidad, integridad y trazabilidad. |

## 📋 Reflexión crítica sobre la coherencia de la arquitectura

En conjunto, la arquitectura propuesta para Zajana S.A.S. muestra un nivel alto de coherencia entre sus diferentes capas. Existe una línea clara que parte de los procesos de negocio, se materializa en entidades de datos concretas, se implementa en aplicaciones orientadas a APIs y se soporta en una infraestructura en la nube diseñada para ser escalable y segura. La vista de seguridad no aparece como un añadido tardío, sino como un componente transversal que se apoya en servicios nativos de Azure (Entra ID, Defender, Sentinel, Purview) y en la alineación con normas del sector financiero, lo que refuerza la consistencia del modelo frente a los requisitos regulatorios.

Sin embargo, la dependencia fuerte de un ecosistema específico (Azure + Snowflake) introduce riesgos de *vendor lock-in* que deben gestionarse mediante contratos, portabilidad de datos y diseño de integraciones lo más desacopladas posible. Adicionalmente, la complejidad de la solución, con múltiples fuentes, APIs y capas analíticas, exige un gobierno de datos y de arquitectura robusto para evitar desalineaciones entre lo que se modela y lo que se implementa. La inclusión del BPMN de migración deja evidencia de que la dimensión organizacional (roles, capacidades del equipo, gestión del conocimiento) es tan crítica como la dimensión técnica. En balance, la arquitectura es coherente y bien alineada con los objetivos del cliente, pero su sostenibilidad en el tiempo dependerá de la capacidad de Zajana para seguir gestionando riesgos, cambios tecnológicos y evolución regulatoria de forma proactiva.

## 🔍 Investigación complementaria
### Tema investigado:
Integración de Vistas Arquitectónicas en el Proceso de Selección de Herramientas de Enterprise Architecture en Philips

### Resumen:
Se presenta el proceso mediante el cual Philips seleccionó una herramienta de Arquitectura Empresarial para apoyar su estrategia corporativa de avanzar “hacia un solo Philips” [1]. La empresa, con presencia global y operaciones altamente fragmentadas, que incluyen más de 100 sistemas ERP diferentes en sus Divisiones de Producto, necesitaba una forma de comprender mejor su estructura y alinear la TI con los objetivos del negocio. Por eso se adoptó el Integrated Architecture Framework (IAF), buscando una herramienta que ofreciera soporte directo al marco IAF, colaboración multiusuario y trazabilidad de decisiones y modelos arquitectónicos [1].

La integración de vistas arquitectónicas fue el eje central de la evaluación. Durante la prueba, la herramienta Metis permitió combinar múltiples Architecture Descriptions:

- Hydra (arquitectura actual de Semiconductores),
- PHERA (arquitectura corporativa común),
- SITAR (estrategias y principios de negocio y TI).

A partir de estas, se creó una cuarta vista basada en el IAF, vinculando objetos y verificando consistencia entre modelos. Este análisis reveló inconsistencias entre Hydra y PHERA y permitió rastrear dependencias entre estrategias y aplicaciones, demostrando cómo la integración de vistas puede apoyar la coherencia corporativa y la toma de decisiones informada en Philips [1].

## 📚 Referencias
- [1] P. Dragstra, Enterprise Architecture: The Selection Process of an Enterprise Architecture Toolset to Support Understanding and Governing the Enterprise, Eindhoven University of Technology, 2005.
---

_Este documento hace parte de la entrega del taller 7 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
