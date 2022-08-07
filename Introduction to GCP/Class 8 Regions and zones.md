in each zone is a datacenter, and you can use a single zone o multiple, that influes in latency, the main idea is to use many zones to protect the application. https://gcping.com/


![[Pasted image 20220807113753.png]]


Regiones y zonas en GCP

-   La región es una zona geográfica donde se encuentran varias zonas separadas por una distancia determinada, en las cuales cada una de estas zonas tienen adentro los data centers.
    
-   Muchas veces vamos a requerir que nuestra aplicación o software este en varias  
    zonas y/o regiones por alta disponibilidad y con latencia, para evitar que una catástrofe ya sea natural o humana altere nuestros servicios.
    
-   Los puntos de presencia son data centers de los proveedores de servicio de internet locales con los que Google tiene contratos y/o convenios