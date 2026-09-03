# MiCita Salud - Sistema de Gestión de Citas Médicas

## Descripción del Proyecto
"MiCita Salud" es una solución integral diseñada para una IPS de Bucaramanga. La plataforma permite a los pacientes (afiliados y particulares) gestionar sus citas médicas, facilita a los médicos el registro de evoluciones clínicas mediante la integración con sistemas HIS y optimiza la administración de agendas y reportes para el personal administrativo.

## Equipo de Desarrollo
- **Erit Santiago Arenas Rangel** - Rol (Diseñador de Software)

## Herramienta de Modelado
Para el diseño de la arquitectura y procesos de este proyecto, se seleccionó **Lucidchart**.

### Justificación de la elección:
La elección se basa en su capacidad de colaboración en la nube y su soporte para el estándar UML 2.5. Comparado con StarUML, Lucidchart ofrece una curva de aprendizaje más baja y una mayor flexibilidad para compartir avances con los interesados de la IPS de forma remota, garantizando que los diagramas de casos de uso y secuencias sean legibles y exportables en alta calidad.

## Identificación de Actores y Casos de Uso (Fase 2)

A partir del análisis del caso de estudio, se han identificado los siguientes elementos clave para el modelado:

### Actores del Sistema
 Actor | Tipo | Rol / Justificación |
**Paciente** | Primario | Inicia las acciones de gestión de citas (General). |
**Paciente Afiliado** | Primario | Especialización del paciente (Cita cubierta por EPS). |
**Paciente Particular** | Primario | Especialización (Debe realizar pago para confirmar). |
**Médico** | Primario | Gestiona su agenda diaria y registra la evolución médica. |
**Auxiliar Adm.** | Primario | Administra agendas globales y genera reportes. |
**Pasarela de Pagos** | Secundario | Sistema externo que procesa cobros de pacientes particulares. |
**Sistema HIS** | Secundario | Repositorio externo de historias clínicas de la institución. |
**Servicio Mensajería** | Secundario | Proveedor externo para notificaciones (SMS/Email). |

### Casos de Uso Principales (CU)
El sistema se compone de funcionalidades clave que incluyen:
**CU-02 Autenticar usuario:** Requisito obligatorio para operaciones sensibles.
**CU-03 Solicitar cita médica:** Proceso principal de agendamiento.
**CU-06 Registrar evolución médica:** Acción realizada por el médico durante la consulta.
**CU-12 Adjuntar resultados:** Funcionalidad opcional (extensión) al solicitar cita.
