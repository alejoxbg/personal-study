


## Identidad y control de acceso

![[Pasted image 20220807150034.png]]

### ¿Quién es el miembro?

Puede ser

-   una **persona**
-   un **subsistema** (ejem. Aplicación): esto se le conoce como _service account_.

**Zero Trust / Confianza Cero**: No confiamos en lo que está dentro de nuestro perímetro de seguridad de forma automática.

-   Las comunicaciones dentro del perímetro de seguridad están cifradas y vienen con permisos.
-   Establecemos que aplicaciones pueden hablar con que aplicaciones.
-   Determinamos el tipo de recursos que las aplicaciones pueden generar.

### ¿Qué puede hacer?

Existe una taxonomía muy grande de recursos relacionados con que puede hacer.

Los recursos tienen ciertos permisos asignados. Además los permisos permiten realizar acciones sobre un recurso:

-   Generar uno nuevo
-   Modificarlo
-   Borrarlo
-   Hacerle update

### ¿En cuál recurso?

Las políticas de seguridad se asignan a cada uno de los recursos. En una política podemos establecer el rol de los miembros.

---

Quién puede hacer qué en cuál recurso.

El quién es persona o aplicación.  
El qué son permisos y se asignan a través de roles.

---

### Roles
![[Pasted image 20220807150331.png]]
Los roles son una colección de permisos detallados que asignamos a grupos.

Podemos generar nuestros propios roles, pero ya hay varios existentes.

### Asignación de politicas y herencia
![[Pasted image 20220807150523.png]]
Se puede asignar a varios niveles: podemos asignar políticas a nivel org. folder, proyecto y recurso.  
Además de que heredan la política de los nodos superiores.

### Estructura de una política

```
{
 "bindings": [
 {
 	"role": "roles/storage.objectAdmin",
	"members": [
		"user:alice@acme.com",
 		"serviceAccount:my-other-app@appspot.gserviceaccount.com",
 		"group:admins@acme.com",
 		"domain:acme.com" ]
 },
 {
 	"role": "roles/storage.objectViewer",	# rol
 	"members": ["user:bob@acme.com"]	# a los que les asignaremos el rol
 }
 ]
}
```