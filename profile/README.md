<div align="center">
  <img src="URL_DE_TU_BANNER_CORPORATIVO.png" alt="MONDRAGON-X" width="100%" />
</div>

<h1 align="center">MONDRAGON-X</h1>

<p align="center">
  <em>Espacio de trabajo y repositorio central del proyecto Mondragon-X. Aquí gestionamos la infraestructura, componentes y casos de uso mediante arquitecturas basadas en contenedores.</em>
</p>

---

## Arquitectura y Organización

Nuestra infraestructura está modularizada y orientada a **Casos de Uso (KITs)**. Para facilitar el despliegue y el mantenimiento, nos organizamos de la siguiente manera:

1. **KITs / Helms:** Cada caso de uso principal se despliega mediante [Helm Charts](https://helm.sh/). Estos repositorios contienen la configuración de orquestación.
2. **Componentes Individuales:** Cada servicio, API, o imagen Docker que forma parte de un Helm tiene **su propio repositorio independiente**. Esto nos permite versionar y actualizar componentes sin afectar al empaquetado general.

> [!WARNING]  
> **Nota para agentes externos:** La mayoría de los repositorios de esta organización son **privados** por políticas corporativas. Si haces clic en un enlace de la lista inferior y recibes un error `404`, significa que no tienes los permisos de lectura asignados.

---

## Catálogo de KITs y Casos de Uso

A continuación, detallamos los principales módulos de nuestro sistema. *(Haz clic en los enlaces para ir al repositorio, requiere acceso corporativo).*

### KIT 1: Espacio de Datos
- **Descripción:** El despliegue de el Espacio de Datos de Mondragon-X.
- **Repositorio Helm:** [`/mondragon-x-umbrella`](https://github.com/mondragon-x/mondragon-x-umbrella)
- **Componentes clave:**
  - [`/landing-page`](https://github.com/mondragon-x/portal-web) - Landing page utilizada para informar a todos los posibles usuarios que ofrece este Espacio de Datos sin proporcionar acceso a el. Ademas, tambien habilita la opcion de comunicarse con el equipo responsable del onboarding de nuevos participantes.
  - [`/portal-assets`](https://github.com/mondragon-x/portal-assets) - Aplicacion que contiene todos los recursos comunes entre aplicaciones.
  - [`/portal-frontend`](https://github.com/mondragon-x/portal-frontend) - Aplicacion que contiene el frontend del portal.
  - [`/portal-frontend-registration`](https://github.com/mondragon-x/portal-frontend-registration) - Aplicacion que contiene el frontend del portal en fase de registro.
  - [`/portal-backend`](https://github.com/mondragon-x/portal-backend) - Aplicacion que contiene el backend del portal

---

## Stack Tecnológico

<div align="center">
  <img src="https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" />
  <img src="https://img.shields.io/badge/helm-%230F1689.svg?style=for-the-badge&logo=helm&logoColor=white" alt="Helm" />
  <img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python" />
  <img src="https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white" alt="C#" />
  <img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/PostgreSQL-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
 <img src="https://img.shields.io/badge/Vault-%23000000.svg?style=for-the-badge&logo=vault&logoColor=white" alt="Vault" />
 <img src="https://img.shields.io/badge/MicroK8s-%23E95420.svg?style=for-the-badge&logo=kubernetes&logoColor=white" alt="MicroK8s" />
 <img src="https://img.shields.io/badge/SeaweedFS-%2320B2AA.svg?style=for-the-badge&logoColor=white" alt="SeaweedFS" />
</div>

---

## Acceso y Contacto

Si eres un proveedor, auditor o agente externo colaborando en este proyecto corporativo y necesitas acceso al código fuente o a los registros de contenedores, por favor sigue estos pasos:

1. Contacta con tu responsable interno del proyecto.
2. Abre un ticket en el repositorio [`/.github`](https://github.com/mondragon-x/.github) solicitando acceso a los repositorios específicos.
3. El equipo revisará y aprobará tu petición.