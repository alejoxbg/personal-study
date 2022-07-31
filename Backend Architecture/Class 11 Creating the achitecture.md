  Aquí se empieza a ver lo que es un sistema distribuido, podemos ver como todo es agnóstico a todo y se unen por comunicación. Cuando hablamos de lectura (POST) recordamos que solo son 10 usuarios que van a estar escribiendo, es por eso que no hacemos tanto énfasis en ello, incluso una base de datos NoSQL puede bastar, ya que realmente se va a estar leyendo muy poco.  
.  
En cambio para la lectura, son mils de usuarios, así que ahí necesitamos tener poder de procesamiento, además de que tenemos que entregar respuesta de manera inmediata. Las bases de datos SQL suelen ser mejor para lectura, ya que con ellas podemos realizar querys complejas y obtener el resultado que deseamos (cosa que no podríamos con una NoSQL, a no ser que suframos)  
.  
De hecho, incluso podríamos tener una tercera base de datos que almacene esos datos que no se está usando y esa base de datos puede ser usada para Machine Learning y Business Intelligence.  
.  
Recomiendo el curso de [Fundamentos de Bases de Datos  
](https://platzi.com/clases/bd/)para profundizar en para qué es bueno cierto tipo de bases de datos.

![[Pasted image 20220731140418.png]]