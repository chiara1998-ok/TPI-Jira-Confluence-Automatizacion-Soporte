# Configuración Propuesta del Chatbot en Jira Service Management

## Objetivo

Automatizar la atención de consultas repetitivas relacionadas con instructivos utilizando Jira Service Management, Confluence y el Agente de Servicio Virtual.

## Paso 1: Crear Base de Conocimiento

1. Crear un espacio en Confluence.
2. Crear una sección denominada "Instructivos".
3. Cargar documentación validada por soporte de manera interna.
4. Mantener actualizados los artículos.

## Paso 2: Configurar Jira Service Management

1. Crear proyecto de soporte.
2. Habilitar Virtual Service Agent y el servicio de Rovo(IA).
3. Asociar el proyecto al espacio de Confluence.
4. Configurar permisos de lectura.

## Paso 3: Flujo de Atención

1. Usuario inicia conversación.
2. El chatbot analiza la consulta.
3. Busca coincidencias en Confluence.
4. Devuelve respuesta e instructivo.
5. Solicita validación.

## Paso 4: Escalamiento

Si:

* No existe documentación.
* La respuesta no resuelve el problema.
* La consulta es ambigua.

Entonces:

* Se crea o actualiza un ticket.
* El caso es asignado al equipo de soporte.

## Estados del Proceso

* ST_ESPERANDO_TICKET
* ST_ANALIZANDO_CONSULTA
* ST_BUSCANDO_CONFLUENCE
* ST_RESPUESTA_ENVIADA
* ST_VALIDANDO_RESPUESTA
* ST_ESCALADO_HUMANO
* ST_RESUELTA
* ST_CERRADA

