# Trabajo Práctico: Implementación de CI/CD con Kubernetes y GitHub Actions

## Objetivo General
Implementar un pipeline de CI/CD completo para una aplicación web utilizando Kubernetes (Minikube), GitHub Actions y Docker Hub, con diferentes ambientes de desarrollo y políticas de aprobación.

## Requisitos Previos
- Conocimientos básicos de Docker y Kubernetes
- Cuenta en GitHub y Docker Hub
- Máquina virtual para hosting (puede ser local o en la nube)

## Entrega 1: Configuración del Ambiente Base
**Objetivo**: Preparar el ambiente de desarrollo y la infraestructura básica.

Tareas:
1. Configurar una máquina virtual con los siguientes componentes:
   - Docker
   - Kubernetes (Minikube)
   - kubectl
   - ngrok
2. Documentar el proceso de instalación y configuración
3. Verificar y demostrar el funcionamiento correcto de cada componente
4. Elaborar un informe con los comandos utilizados y capturas de pantalla

## Entrega 2: Containerización de la Aplicación
**Objetivo**: Preparar la aplicación para su despliegue en Kubernetes.

Tareas:
1. Crear cuenta en Docker Hub
2. Escribir el Dockerfile para la aplicación proporcionada
3. Construir la imagen y subirla a Docker Hub
4. Probar la imagen localmente
5. Documentar el proceso y las decisiones tomadas

## Entrega 3: Configuración de Kubernetes
**Objetivo**: Crear los manifiestos necesarios para el despliegue en Kubernetes.

Tareas:
1. Crear los siguientes manifiestos de Kubernetes:
   - Deployment (con 3 réplicas)
   - Service
   - Ingress
   - ConfigMaps y Secrets necesarios
2. Crear estructura de directorios para múltiples ambientes (dev/staging/prod)
3. Implementar Kustomize para manejar las diferencias entre ambientes
4. Probar el despliegue en Minikube
5. Documentar la estructura y explicar cada componente

## Entrega 4: Exposición del Servicio
**Objetivo**: Hacer la aplicación accesible desde Internet.

Tareas:
1. Configurar ngrok para exponer el servicio
2. Documentar el proceso de exposición
3. Implementar y documentar medidas de seguridad básicas
4. Probar y verificar el acceso desde Internet
5. Proporcionar ejemplos de uso

## Entrega 5: Implementación de CI/CD
**Objetivo**: Crear un pipeline completo de CI/CD con GitHub Actions.

Tareas:
1. Crear repositorio en GitHub con la estructura apropiada
2. Configurar los siguientes workflows de GitHub Actions:
   - Pipeline para desarrollo
   - Pipeline para staging
   - Pipeline para producción
3. Implementar políticas de branch protection
4. Configurar requerimientos de PR y aprobaciones
5. Documentar el proceso completo

## Entrega 6: Gestión de Secretos
**Objetivo**: Implementar un manejo seguro de secretos y configuraciones sensibles.

Tareas:
1. Configurar secrets en GitHub Actions
2. Implementar manejo de secretos en Kubernetes
3. Documentar las mejores prácticas implementadas
4. Realizar pruebas de seguridad básicas
5. Proporcionar guía de mantenimiento de secretos

## Criterios de Evaluación
- Funcionalidad (30%)
- Documentación (20%)
- Seguridad (20%)
- Buenas prácticas (15%)
- Presentación y claridad (15%)

## Entrega Final
Presentación del proyecto que incluya:
1. Repositorio en GitHub con todo el código
2. Documentación completa en el README
3. Guía de despliegue y mantenimiento
4. Video demostrativo del pipeline completo
5. Presentación oral del proyecto
6. Informe de lecciones aprendidas y desafíos encontrados

## Bonus Points
- Implementación de monitoreo
- Configuración de alerts
- Implementación de auto-scaling
- Implementación de estrategias de backup
- Implementación de tests automatizados

## Restricciones
- Debe usarse la aplicación proporcionada
- Mínimo 3 réplicas por ambiente
- Debe implementarse en los tres ambientes (dev/staging/prod)
- Debe requerir aprobación para deploy a producción
- Los secretos no deben estar en el código

## Tiempo de Entrega
- 6 semanas totales
- 1 semana por entrega
- Presentación final en la semana 6

¿Te gustaría que detalle algún aspecto específico de alguna de las entregas o que agregue algún criterio adicional de evaluación?