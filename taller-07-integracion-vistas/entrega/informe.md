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
- Cómo se estructura el modelo entregado
- Cómo representa las necesidades del cliente
- Qué supuestos se tomaron

## 📈 Diagrama final entregado

[https://github.com/MariSalas23/AREM-Wiki/wiki/Integraci%C3%B3n-de-Vistas-%E2%80%90-Zajana-S.A.S.](https://github.com/MariSalas23/AREM-Wiki/wiki/Integraci%C3%B3n-de-Vistas-%E2%80%90-Zajana-S.A.S.)

## 📋 Reflexión

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Ej: Paciente        | Actor | Usuario que agenda una cita médica | Cliente |

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
