
# 

**Acerca de arc42**

arc42, La plantilla de documentación para arquitectura de sistemas y de
software.

Por Dr. Gernot Starke, Dr. Peter Hruschka y otros contribuyentes.

Revisión de la plantilla: 7.0 ES (basada en asciidoc), Enero 2017

© Reconocemos que este documento utiliza material de la plantilla de
arquitectura arc42, <https://www.arc42.org>. Creada por Dr. Peter
Hruschka y Dr. Gernot Starke.

# Introducción y Metas
# 1. Introducción y Objetivos

## Objetivo del Sistema ERP
El sistema ERP tiene como objetivo integrar y automatizar los procesos empresariales, permitiendo la gestión eficiente de compras, inventarios, proveedores y productos, mejorando la trazabilidad y control de la información.

## Objetivo del Módulo de Compras
El módulo de compras permite gestionar proveedores, registrar órdenes de compra, controlar la adquisición de productos y garantizar la disponibilidad de inventario.

## Vista de Requerimientos 
## Requisitos de Negocio Principales
- Registrar y gestionar proveedores.
- Crear y administrar órdenes de compra.
- Registrar productos adquiridos.
- Consultar historial de compras.
- Generar reportes de compras.
- Controlar el estado de las órdenes (pendiente, aprobada, recibida).

## Metas de Calidad 
## Metas de Calidad

- Usabilidad: El sistema debe ser fácil de usar por el personal de compras.
- Rendimiento: Las consultas deben responder en menos de 2 segundos.
- Seguridad: Acceso controlado mediante autenticación y roles.
- Escalabilidad: Permitir agregar nuevos módulos en el futuro.

## Partes interesadas (Stakeholders)

| Rol            | Contacto                  | Expectativas                              |
|----------------|---------------------------|------------------------------------------|
| Administrador  | admin@empresa.com         | Control total del sistema                |
| Compras        | compras@empresa.com       | Gestionar proveedores y órdenes de compra|
| Gerencia       | gerente@empresa.com       | Reportes y métricas del sistema          |


# Restricciones de la Arquitectura 
# Restricciones de la Arquitectura

- Backend desarrollado en Java con Spring Boot.
- Base de datos PostgreSQL.
- Frontend desarrollado en React (SPA).
- Comunicación mediante API REST.
- Despliegue usando Docker.
- El sistema debe ser accesible vía navegador web.


# Alcance y Contexto del Sistema 
## Contexto de Negocio

El sistema ERP interactúa con usuarios internos (personal de compras y administradores) y proveedores externos.


**\<optionally: Explanation of external domain interfaces\>**

## Contexto Técnico {#_contexto_técnico}

**\<Diagrama o Tabla\>**

**\<Opcional: Explicación de las interfases técnicas\>**

**\<Mapeo de Entrada/Salida a canales\>**

# Estrategia de solución 

# Vista de Bloques 
### Bloques de Construcción

- Frontend Web (React): Interfaz para usuarios.
- Backend API (Spring Boot): Lógica de negocio.
- Base de Datos PostgreSQL: Almacenamiento de datos.
- Servicio de Autenticación: Gestión de usuarios y roles.

## Sistema General de Caja Blanca {#_sistema_general_de_caja_blanca}

***\<Diagrama general\>***

Motivación

:   *\<Explicación en texto\>*

Bloques de construcción contenidos

:   *\<Desripción de los bloques de construcción contenidos (Cajas
    negras)\>*

Interfases importantes

:   *\<Descripción de las interfases importantes\>*

### \<Caja Negra 1\> {#_caja_negra_1}

*\<Propósito/Responsabilidad\>*

*\<Interfase(s)\>*

*\<(Opcional) Características de Calidad/Performance\>*

*\<(Opcional) Ubicación Archivo/Directorio\>*

*\<(Opcional) Requerimientos Satisfechos\>*

*\<(Opcional) Riesgos/Problemas/Incidentes Abiertos\>*

### \<Caja Negra 2\> {#_caja_negra_2}

*\<plantilla de caja negra\>*

### \<Caja Negra N\> {#_caja_negra_n}

*\<Plantilla de caja negra\>*

### \<Interfase 1\> {#_interfase_1}

...​

### \<Interfase m\> {#_interfase_m}

## Nivel 2 {#_nivel_2}

### Caja Blanca *\<bloque de construcción 1\>* {#_caja_blanca_bloque_de_construcción_1}

*\<plantilla de caja blanca\>*

### Caja Blanca *\<bloque de construcción 2\>* {#_caja_blanca_bloque_de_construcción_2}

*\<plantilla de caja blanca\>*

...​

### Caja Blanca *\<bloque de construcción m\>* {#_caja_blanca_bloque_de_construcción_m}

*\<plantilla de caja blanca\>*

## Nivel 3 {#_nivel_3}

### Caja Blanca \<\_bloque de construcción x.1\_\> {#_caja_blanca_bloque_de_construcción_x_1}

*\<plantilla de caja blanca\>*

### Caja Blanca \<\_bloque de construcción x.2\_\> {#_caja_blanca_bloque_de_construcción_x_2}

*\<plantilla de caja blanca\>*

### Caja Blanca \<\_bloque de construcción y.1\_\> {#_caja_blanca_bloque_de_construcción_y_1}

*\<plantilla de caja blanca\>*

# Vista de Ejecución {#section-runtime-view}

## Escenario de ejecución: Registrar Producto


### Flujo
1. El usuario ingresa los datos del producto en el frontend.
2. El frontend envía la solicitud al backend.
3. El backend valida los datos.
4. El backend guarda el producto en la base de datos.
5. Se devuelve confirmación al usuario.




## Nivel de infraestructura 1 {#_nivel_de_infraestructura_1}

***\<Diagrama General\>***

Motivación

:   *\<Explicación en forma textual\>*

Características de Calidad/Rendimiento

:   *\<Explicación en forma textual\>*

    Mapeo de los Bloques de Construcción a Infraestructura

    :   *\<Descripción del mapeo\>*

## Nivel de Infraestructura 2 {#_nivel_de_infraestructura_2}

### *\<Elemento de Infraestructura 1\>* {#_elemento_de_infraestructura_1}

*\<diagrama + explicación\>*

### *\<Elemento de Infraestructura 2\>* {#_elemento_de_infraestructura_2}

*\<diagrama + explicación\>*

...​

### *\<Elemento de Infraestructura n\>* {#_elemento_de_infraestructura_n}

*\<diagrama + explicación\>*

# Conceptos Transversales (Cross-cutting) {#section-concepts}

## *\<Concepto 1\>* {#_concepto_1}

*\<explicación\>*

## *\<Concepto 2\>* {#_concepto_2}

*\<explicación\>*

...​

## *\<Concepto n\>* {#_concepto_n}

*\<explicación\>*

# Decisiones de Diseño {#section-design-decisions}

# Requerimientos de Calidad {#section-quality-scenarios}

## Árbol de Calidad {#_árbol_de_calidad}

## Escenarios de calidad {#_escenarios_de_calidad}

# Riesgos y deuda técnica {#section-technical-risks}
# Vista de Despliegue

El sistema se desplegará en un servidor usando contenedores Docker.

- Contenedor Backend Spring Boot
- Contenedor PostgreSQL
- Servidor Web React
- Nginx como proxy inverso

# Glosario {#section-glossary}
# Glosario

| Término        | Definición |
|----------------|------------|
| Producto       | Bien adquirido o vendido por la empresa |
| Proveedor      | Persona o empresa que suministra productos |
| Orden de Compra| Documento que autoriza la compra |
| ERP            | Sistema de planificación de recursos empresariales |
| Inventario     | Productos almacenados |
| Usuario        | Persona que usa el sistema |


