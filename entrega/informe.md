# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 7 - Integración de Vistas de Arquitectura_

## 👥 Integrantes del equipo
- Juan David Cetina Gómez (juancego@unisabana.edu.co)
- Ana Lucía Quintero Vargas (anaquiva@unisabana.edu.co)
- Mariana Salas Gutiérrez (marianasalgu@unisabana.edu.co)

## 🧠 Descripción general del trabajo
Describa brevemente el objetivo del taller y cómo se desarrolló la actividad.

## 🔧 Proceso de desarrollo
Explique cómo realizaron el trabajo: qué decisiones tomaron, qué herramientas utilizaron, qué aspectos modelaron primero y cómo lo fueron ajustando.

## 🧩 Análisis del modelo propuesto
Incluya un análisis sobre:
- Cómo se estructura el modelo entregado
- Cómo representa las necesidades del cliente
- Qué supuestos se tomaron

## 📈 Diagrama final entregado
> (Inserte aquí una imagen o enlace al modelo-final.drawio / .asta / PDF)

## 📋 Tabla de actores, entidades o componentes (si aplica)

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Ej: Paciente        | Actor | Usuario que agenda una cita médica | Cliente |

## 🔍 Investigación complementaria
### Tema investigado:
ArchiMate

### Resumen:
ArchiMate es un lenguaje visual estandarizado orientado a la Arquitectura Empresarial, creado por The Open Group. Su propósito es representar, analizar y mostrar de manera coherente cómo se relacionan los distintos elementos de una organización, desde los procesos del negocio hasta las soluciones tecnológicas que los soportan [1]. Puede ser altamente complejo, ArchiMate incorpora viewpoints, entendidos como guías o convenciones que permiten generar vistas parciales del modelo para atender inquietudes específicas de diferentes interesados. La especificación se estructura en capas, aplicación y tecnología, además estructura activa, comportamiento y estructura pasiva, lo que posibilita construir una perspectiva integral de la organización. Gracias a esta estructura multinivel, ArchiMate funciona como un lenguaje de descripción de alto nivel que puede enlazarse con otros lenguajes más detallados, por ejemplo UML para modelado de software o BPMN para la descripción de procesos, añadiendo precisión donde sea necesario [1]. ArchiMate aporta la claridad visual indispensable para soportar la formulación e implementación de las hojas de ruta estratégicas de la AE.

La integración de vistas arquitectónicas dentro de ArchiMate se basa en la definición de correspondencias y reglas de transformación hacia otros lenguajes ubicados en distintos niveles de abstracción. Una investigación académica desarrolló un mecanismo para incorporar requerimientos de seguridad desde la capa de negocio de ArchiMate hasta la capa de interfaz de usuario, empleando la extensión BPMN-BPSec y el lenguaje IFML. Este proceso requirió identificar equivalencias entre los requisitos de seguridad definidos en ArchiMate y los representados en BPMN-BPSec, considerando las relaciones contextuales entre los elementos para asegurar una correspondencia modelo a modelo, más allá de simples equivalencias puntuales [2]. En el marco de la Arquitectura Dirigida por Modelos (MDA), la capa de negocio de ArchiMate y BPMN se ubican en el nivel de Modelo Independiente de la Computación, lo que permitió formular reglas de transformación automáticas que habilitan una correspondencia C2C entre ArchiMate y BPMN-BPSec [2]. Estas transformaciones evidencian que es viable mantener la trazabilidad y alineación de los objetivos de seguridad del negocio dentro de las soluciones de TI.

## 📚 Referencias
- [1] The Open Group, ArchiMate 101: A Practical Introduction.
- [2] Universidad del Bío-Bío, Tesis de Magíster en Ciencias de la Computación.

---

_Este documento hace parte de la entrega del taller 7 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
