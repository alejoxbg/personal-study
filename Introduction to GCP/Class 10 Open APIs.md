In many cases is really difficult to migrate your applications, data, etc to another provider, with GCP is really easy and is because GCP use something called Hybrid Cloud, Is a composition of 2 or more clouds, private, comunitary or public that offer you multiple benefits and implementation models. haven GCP-AWS-Azure, learn this is very difficult and there are different software that help to do this.

Google is the pioneer in this industry ans Anthos is a lot o patters of design to desing our system.

![[Pasted image 20220807121704.png]]


![[Pasted image 20220807121808.png]]

![[Pasted image 20220807121818.png]]

![[Pasted image 20220807121856.png]]

Big Query is an example of that, it can load 1 Petabyte per second, the query splits in a lot of pieces that process paralell queryes.

#### BigQuery: patrones en la nube

Como BigQuery aprovecha la infraestructura de la nube para trabajar de forma paralela y darnos resultados.

1.  Mandamos query en SQL.
2.  Punto de presencia: entra a la red de Google.
3.  Llegar al DataCenter más cercano, viajando por la _private fiber network_ de Google.
4.  La query se encamina a un cluster dentro del data center. Podemos tener anchos de banda muy potentes como 1 _petabyte_ por segundo de datos.
5.  Un nodo ejecutador convierte nuestra query en un plan ejecutador; es decir, divide nuestra query en pedacitos para procesarlos de manera paralela.
6.  Escogen máquinas que ejecutarán nuestros pedacitos de query de forma paralela.
7.  El resultado se junta y se regresa al usuario.




