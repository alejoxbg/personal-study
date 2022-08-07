

## Roles de IAM

---
![[Pasted image 20220807151256.png]]
-   User
-   Group
    -   Role
    -   Resource

Grupos a nivel de organización
![[Pasted image 20220807151753.png]]
-   Super Administradores
    -   igual al super usuario de Linux
    -   es un usuario con un montón de poderes
-   Org. Admins
    -   Define politicas de IAM
    -   Determina la estructura de la jerarquía de recursos
    -   Crea proyectos hasta que la organización este madura
-   Network Admins
    -   Crea redes, subredes, dispositivos de red (enrutadores en la nube, VPN en la nube y balanceadores de carga en la nube)
    -   Mantiene las reglas del firewall, a menos que las mantenga el administrador de seguridad
-   Security Admins
    -   Establece políticas y restricciones para toda la organización, carpetas y proyectos
    -   Establece roles de IAM para proyectos
    -   Mantiene la visibilidad de los logs y los recursos
-   Billing Admins
    -   Configura una cuenta de facturación
    -   Monitorear el uso de los recursos