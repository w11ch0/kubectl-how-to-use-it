# kubectl-how-to-use-it
En Kubernetes, cada administrador necesita una herramienta confiable. Kubectl get nodes, es el comando que revela las bondades de un clúster.

¿Qué es Kubectl Get Nodes y cómo usarlo?

En Kubernetes, cada administrador necesita una herramienta confiable para navegar por la compleja red de nodos. Ingrese kubectl get nodes, el último comando que revela los secretos de su clúster. 

La introducción del kubectl get nodescomando en el ecosistema de línea de comandos de Kubernetes fue impulsada por la necesidad de que los administradores y desarrolladores recuperaran información sobre los nodos del clúster. 

En este blog, lo guiaremos a través de los conceptos básicos de este comando, ayudándolo a obtener la confianza y la experiencia para navegar y administrar su entorno de Kubernetes como un profesional. ¡Prepárese para tomar el control de sus clústeres con facilidad!

¡Sumerjámonos y desbloqueemos el potencial de este comando indispensable!


Cubriremos:

¿Qué es kubectl get nodes?
¿Cómo correr kubectl get nodes?
¿ Cuándo usar kubectl to get nodes?
Kubectl obtiene etiquetas de nodo
Kubectl obtener nodo para pods
Casos de uso dekubectl get nodes

## ¿Qué hace kubectl get nods?


kubectl get nodeses un comando poderoso que proporciona información esencial sobre los nodos en su clúster de Kubernetes. Cuando ejecuta este comando, se comunica con el servidor API de Kubernetes, recuperando la información necesaria del plano de control del clúster. 

El kubectl get nodescomando obtiene el estado actual de todos los nodos del clúster y muestra la información en un formato tabular, como se muestra a continuación.

<sub>$ kubectl get nodes</sub>

Output:

NAME       STATUS   ROLES    AGE     VERSION
node-1     Ready    <none>   7d      v1.21.3
node-2     Ready    <none>   7d      v1.21.3
node-3     Ready    <none>   7d      v1.21.3
Las columnas de salida que se obtienen son:

NOMBRE : El nombre del nodo dentro del clúster.
ESTADO : el estado actual del nodo, que indica si está listo, no listo o inalcanzable.
ROLES : cualquier rol asignado al nodo, como maestro, trabajador, etc.
EDAD : la duración desde que se creó o agregó el nodo al clúster.
VERSIÓN : la versión de Kubernetes se está ejecutando en el nodo.
INTERNAL-IP : La dirección IP interna asignada al nodo.
EXTERNAL-IP : la dirección IP externa asignada al nodo, si corresponde.
Este comando proporciona una descripción general rápida de los nodos del clúster, brindándonos la información para monitorear aún más la infraestructura de Kubernetes. A menudo se usa para la resolución de problemas, el escalado, la planificación de la capacidad y las tareas generales de administración de clústeres .
