# Despliegue de plataforma de microservicios con Kubernetes

Tu empresa necesita desplegar una plataforma de microservicios en Kubernetes para mejorar la escalabilidad y resiliencia de sus aplicaciones. La plataforma debe soportar despliegues continuos con Helm y GitOps utilizando ArgoCD, y debe ser monitoreada con Prometheus y Grafana. Los servicios deben ser desplegados en un clúster de Kubernetes gestionado en la nube. Los microservicios incluyen un servicio de autenticación, un servicio de usuario y un servicio de pedidos. El sistema debe manejar al menos 10 000 solicitudes por segundo con un tiempo de respuesta promedio menor a 500ms. Debes asegurar la alta disponibilidad y tolerancia a fallos de los servicios.

## Informacion General

| Campo | Valor |
|-------|-------|
| **Tema** | kubernetes-devops |
| **Nivel** | advanced-l2 |
| **Tipo** | practical |
| **Tiempo estimado** | 4 horas |

## Fases del Reto

### Fase 0: Configuración del Proyecto

**Objetivo:** Obtener el proyecto base funcional enviando el Código Base a un asistente de IA, que lo analizará, corregirá errores y generará un ZIP listo para usar.

**Tiempo estimado:** 15-30 minutos

**Instrucciones:**

- Asegúrate de tener instalado para ejecutar el proyecto: Un IDE o editor de código.
- Copia todo el contenido del campo **Código Base** de este reto — incluyendo el texto de instrucciones que aparece al inicio.
- Abre un asistente de IA (Claude en claude.ai, ChatGPT o Gemini — se recomienda Claude), pega el contenido copiado en el chat y envíalo.
- El asistente analizará los archivos, corregirá errores y generará un archivo ZIP descargable. Descárgalo y extráelo en la carpeta donde quieras trabajar.
- Verifica que el proyecto arranca sin errores.

**Entregable:** El proyecto compila/arranca sin errores.

<details>
<summary>Pistas de conocimiento</summary>

- Copia el Código Base completo incluyendo el texto de instrucciones al inicio — esas instrucciones le indican al asistente exactamente qué hacer con los archivos.
- Si el asistente no genera el ZIP automáticamente al terminar el análisis, escríbele: "genera el ZIP ahora".
- Si el proyecto tiene errores al arrancar, comparte el mensaje de error con el mismo asistente para que lo corrija.

</details>

### Fase 1: Configuración del clúster de Kubernetes

**Objetivo:** Tenga un clúster de Kubernetes configurado y operativo en la nube.

**Tiempo estimado:** 1 hora

**Instrucciones:**

- Selecciona un proveedor de nube y crea un clúster de Kubernetes.
- Configura las redes y el almacenamiento necesarios para los microservicios.
- Verifica que el clúster esté funcionando correctamente.

**Entregable:** Clúster de Kubernetes configurado y operativo.

<details>
<summary>Pistas de conocimiento</summary>

- Considera la escalabilidad y la tolerancia a fallos al configurar el clúster.
- Revisa las mejores prácticas para la seguridad del clúster.

</details>

### Fase 2: Despliegue de microservicios con Helm

**Objetivo:** Despliega los microservicios de autenticación, usuario y pedidos utilizando Helm.

**Tiempo estimado:** 1 hora

**Instrucciones:**

- Crea los charts de Helm para cada microservicio.
- Despliega los microservicios en el clúster de Kubernetes.
- Verifica que los microservicios estén funcionando correctamente.

**Entregable:** Microservicios desplegados y operativos en Kubernetes.

<details>
<summary>Pistas de conocimiento</summary>

- Utiliza valores de Helm para parametrizar la configuración de los microservicios.
- Asegura que los microservicios estén correctamente conectados entre sí.

</details>

### Fase 3: Implementación de GitOps con ArgoCD

**Objetivo:** Configura ArgoCD para gestionar los despliegues de los microservicios.

**Tiempo estimado:** 1 hora

**Instrucciones:**

- Instala y configura ArgoCD en el clúster de Kubernetes.
- Configura los repositorios de Git para los microservicios.
- Verifica que ArgoCD esté gestionando los despliegues de los microservicios.

**Entregable:** ArgoCD configurado y gestionando los despliegues de los microservicios.

<details>
<summary>Pistas de conocimiento</summary>

- Utiliza ArgoCD para sincronizar automáticamente los cambios en los microservicios.
- Asegura que ArgoCD esté configurado para notificar cambios y errores.

</details>

### Fase 4: Monitoreo con Prometheus y Grafana

**Objetivo:** Configura Prometheus y Grafana para monitorear los microservicios.

**Tiempo estimado:** 1 hora

**Instrucciones:**

- Instala y configura Prometheus en el clúster de Kubernetes.
- Configura los scrapes de Prometheus para los microservicios.
- Instala y configura Grafana para visualizar los datos de Prometheus.
- Crea dashboards en Grafana para monitorear los microservicios.

**Entregable:** Prometheus y Grafana configurados y monitoreando los microservicios.

<details>
<summary>Pistas de conocimiento</summary>

- Utiliza Prometheus para recolectar métricas de los microservicios.
- Crea alertas en Prometheus para notificar errores y problemas.
- Utiliza Grafana para visualizar las métricas y crear dashboards informativos.

</details>

## Dimensiones Evaluadas

- **queEs**: ¿Qué es Kubernetes y por qué se utiliza para desplegar microservicios?
- **paraQueSirve**: ¿Para qué sirve Helm en el despliegue de microservicios?
- **comoSeUsa**: ¿Cómo se utiliza ArgoCD para implementar GitOps en el despliegue de microservicios?
- **erroresComunes**: ¿Cuáles son los errores comunes al configurar Prometheus y Grafana para monitorear microservicios?
- **queDecisionesImplica**: ¿Qué decisiones implica el diseño de una plataforma de microservicios con Kubernetes?

## Criterios de Evaluacion

- Configurar un clúster de Kubernetes en la nube.
- Desplegar microservicios utilizando Helm.
- Implementar GitOps con ArgoCD.
- Configurar monitoreo con Prometheus y Grafana.

---

*Reto generado automaticamente por Challenge Generator - Pragma*
