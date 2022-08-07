







![[Pasted image 20220807144059.png]]

## La jerarquía de recursos en Google Cloud

-   Mapea la estructura organizacional.
-   Administra a escala.
-   Separación.
-   Herencia de políticas.

#### Organización

Es raíz de la jerarquía de recursos. Esta tiene varias cosas asignadas directamente a la organización:

-   La Billing Account está asignada a esta.
-   Los grupos administradores puede operar en este nodo.
-   Los permisos que toda la organización deba tener se pueden asignar aquí, y heredarlos a los nodos que están debajo.

<h5>Cloud Identity</h5>

Si usamos Google Workspace, el SaaS (Software as a Service) de Google, las identidades son una forma de autenticar a los usuarios que pertenecen a tu organización y tienen acceso a tu Google Cloud.

Cloud Identity nos permite generar los usuarios para Google Cloud sin necesidad de tener Google Workspace. Nos da 50 identidades sin costo.

A la organización se le liga un dominio para identificarla.

#### Folders

Modela la estructura organizacional con GCP (ya sean departamentos, equipos, aplicaciones, cargas de trabajo, ciclo de vida, facturación y aislamiento de seguridad).

Los folders pueden contener proyectos y carpetas.

Poder agrupar las estructuras en folders nos permite:

-   Limitar el acceso, crear grupos y darles permisos en un espacio específico.
-   Discriminar costos, saber cuanto me cuesta un nodo en específico.

#### Proyectos

Contienen los recursos computacionales. Un proyecto es un agrupador de recursos.

Es importante desarrollar un proyecto con una necesidad en mente.  
Ejem:

-   Proyecto de CI/CD
-   Proyecto de un Micro servicio
-   Proyecto para el sitio de marketing

Ventajas de los proyectos pequeños:

-   Fácil mantenimiento
-   Más seguridad
-   Facilidad de Evolución