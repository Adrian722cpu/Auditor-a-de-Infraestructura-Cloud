# Auditoria de Infraestructura Cloud
1. ¿Cuántas líneas de código habéis ahorrado al usar grupos?
Una vez terminada la refactorización, lo que hemos ahorrado sobre todo es reducir la redundancia y permitir que el código sea más fácil de modificar en el tiempo. Esto lo notaremos sobre todo a la hora de querer modificar un dato por ejemplo algo de la CPU o RAM, sabemos que tenemos que acudir al grupo de Hardware por lo que nos ahorrara mucho tiempo futuro. Además al usar un grupo, hemos ahorrado unas 15-20 líneas en definiciones.

2. ¿Qué error os da VS Code si intentáis poner dos servidores con el mismo ID?
Si intento poner la misma IP para dos servidores distintos me aparece el error cvc-identity-constraint.4.1: Duplicate unique value [srv-web-01] found for identity constraint "UnicoID" of element "catalogo_cloud, lo que me hace ver que esta funcionando la restricción unique que he establecido previamente.
