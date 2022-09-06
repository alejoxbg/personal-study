![[Pasted image 20220826230525.png]]

![[Pasted image 20220826231207.png]]

## Sobre Cloud NAT

Es un servicio administrado distribuido definido por software. No se basa en dispositivos o máquinas virtuales proxy.

Cloud NAT configura el software de Andromeda que alimenta nuestra VPC para que proporcione traducción de direcciones de red de origen (NAT de origen o SNAT) para máquinas virtuales sin direcciones IP externas. También proporciona traducción de direcciones de red de destino (NAT de destino o DNAT) para paquetes de respuesta entrantes establecidos.

### Beneficios

**Seguridad**

Puede reducir la necesidad de máquinas virtuales individuales para que cada una tenga direcciones IP externas. Sujeto a las reglas del firewall de salida, las VM sin direcciones IP externas pueden acceder a destinos en Internet. Por ejemplo, es posible que tenga máquinas virtuales que solo necesiten acceso a Internet para descargar actualizaciones o completar el aprovisionamiento.

**Disponibilidad**

Cloud NAT es un servicio administrado distribuido definido por software. No depende de ninguna máquina virtual en su proyecto o de un solo dispositivo de puerta de enlace físico. Configura una puerta de enlace NAT en un Cloud Router, que proporciona el plano de control para NAT y contiene los parámetros de configuración que usted especifica. Google Cloud ejecuta y mantiene procesos en las máquinas físicas que ejecutan sus VM de Google Cloud.

**Escalabilidad**

Cloud NAT se puede configurar para escalar automáticamente la cantidad de direcciones IP de NAT que usa, y admite VM que pertenecen a grupos de instancias administrados, incluidos aquellos con ajuste de escala automático habilitado.

**Rendimiento**

Cloud NAT no reduce el ancho de banda de la red por VM. Cloud NAT es implementado por la red definida por software Andromeda de Google.