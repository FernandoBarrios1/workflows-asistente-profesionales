# workflows-asistente-profesionales
Agente MyF - Sistema Automatizado de Gestión de Citas y Clientes

Este repositorio contiene los flujos de automatización y configuraciones de Agente MyF, un sistema diseñado para automatizar la gestión de clientes, agendamiento de citas, envío de recordatorios y reportes para entornos profesionales y comerciales.

📋 Descripción General

Agente MyF es una solución basada en flujos de trabajo (workflows) que integra bases de datos, plataformas de mensajería/web y sistemas de agendamiento. Su objetivo principal es optimizar la atención al cliente, reducir las ausencias en citas programadas y facilitar el seguimiento contable/operativo mediante reportes periódicos.

🛠️ Arquitectura y Flujos del Sistema

El proyecto se divide en módulos que gestionan aspectos específicos del proceso:

1. Gestión de Clientes

Consultar Clientes: Búsqueda y validación de la información de clientes existentes.

Registrar Clientes: Alta de nuevos usuarios en el sistema.

Actualizar Clientes: Modificación de datos personales o de contacto.

2. Gestión de Agendamientos y Citas

Consultar Disponibilidad: Verificación de horarios libres en la agenda.

Registrar Agendamiento: Creación y confirmación de nuevas citas.

Actualizar / Reagendar Citas: Reprogramación flexible de turnos.

Cancelar Agendamiento: Liberación de horarios previa cancelación del usuario.

Consultar Agendamientos: Historial y estado actual de reservas.

3. Automatizaciones y Notificaciones

Recordatorios de Citas (24h Antes): Notificaciones automáticas previas para reducir el ausentismo.

Agenda Diaria Profesional: Resumen diario enviado al profesional sobre los compromisos del día.

Reporte Mensual de Citas: Generación automática de estadísticas e historial mensual de atención.

Núcleo Agente MyF & Manejo de Errores: Módulos centrales de enrutamiento y control de excepciones para garantizar la estabilidad del sistema.

📂 Estructura del Repositorio

Agente MyF/
├── UT Agente MyF/
│   └── Agenda Diaria Profesional_v2.json
├── Actualizar Agendamiento_v2.json
├── Actualizar Clientes_v2.json
├── Agente MyF_v2.json
├── Cancelar Agendamiento_v2.json
├── Consultar Agendamientos_v2.json
├── Consultar Clientes_v2.json
├── Consultar Disponibilidad_v2.json
├── Manejo de Errores_v2.json
├── MyF Web_v2.json
├── Núcleo Agente MyF_v2.json
├── Reagendar_v2.json
├── Recordatorios de Citas - 24 Horas Antes_v2.json
├── Registrar Agendamiento_v2.json
├── Registrar Clientes_v2.json
└── Reporte Mensual de Citas_v2.json


🚀 Requisitos e Instalación

Prerrequisitos

Una instancia de n8n (versión recomendada v1.0.0 o superior) o motor compatible de ejecución de JSON.

Credenciales configuradas para:

Servicio de mensajería/notificaciones (WhatsApp / Telegram / Email / SMS).

Base de datos o Hoja de Cálculo (Google Sheets, Airtable, PostgreSQL, etc.).

Calendario (Google Calendar, Outlook Calendar, etc.).

Pasos para Importar

Clona o descarga este repositorio:

git clone https://github.com/tu-usuario/agente-myf.git


Accede a tu interfaz de administración de flujos (ej. n8n).

Selecciona Import from File (Importar desde archivo) y carga cada uno de los archivos .json según el módulo que desees desplegar.

Asigna las credenciales correspondientes a cada nodo dentro de la interfaz.

Activa los flujos y verifica el canal de activación (Webhooks, Triggers de tiempo o Eventos).

🔒 Consideraciones de Seguridad y Privacidad

Por motivos de seguridad, no se incluyen tokens de API, contraseñas ni claves secretas en los archivos JSON de este repositorio. Las credenciales deben ser vinculadas localmente dentro del entorno donde se ejecuten los flujos.

🎓 Autoría y Tesis

Este desarrollo forma parte del proyecto de tesis de grado presentado para la carrera de Ingeniería en Informática en la Universidad del Norte sede Asunción. 

Autores: Fernando Barrios, Matías Cáceres 
 
Año: 2026
