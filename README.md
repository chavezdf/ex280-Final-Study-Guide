Partiendo del principio de que este examen esta orientado a administradores y no a desarrolladores, me centrare en organizarlo segun este punto de vista.

# Administracion General de la plataforma
# 1. Verificacion de Plataforma & Troubleshooting
- Listar Nodos
- Listar consumo de recursos en nodos
- Verificar cada nodo
- Projectos Importantes a tomar en cuenta y verificar
- Acceder a Logs de Nodos
- Acceder en modo Debug a un Nodo
- Verificar Status de servicio de Kubelet, Cri-o
- Verificar openvswitch pod

# 2. Configuracion Inicial de la Plataforma
- Agregar un Htpasswd Identity Manager
- Administracion de Usuarios y Permisos
	- Agregar usuarios
		- Asignar cluster-admin a un usuario para dejar de usar kubeadmin
	- Crear grupos y asignar Permisos
		- Asignar permisos para creacion de projectos
		- Quitar al resto los permisos para crear proyectos
		- Asignar permisos de edicion para los desarrolladores
		- Asignar permisis de vista para los testers
- Configuracion de plantilla para proyectos
	- Agregar Network Policies
		- Ayuda: https://access.redhat.com/documentation/en-us/openshift_container_platform/4.5/html-single/networking/index
		- Seccion: Networking - Tema 9.
	- Agregar LimitRanges
	- Agregar Quotas
- Configurar Regiones y Zonas para el Scheduling
	- Etiquetar Nodos
	- Establecer Tains si son necesarios

# 3. Manejo de Projectos
- Creacion de proyectos y apps
- Creacion de Service Accounts
- Asignacion de Service Accounts a Deployment/DC
- Creacion de rutas no seguras y seguras
	- Crear Certificados con openssl
- Creacion de Secrets
- Creacion de Config Maps
- Creacion de PVC
- Montar volumenes
Manejar el Scheduling
- Asignar etiquetas a los proyectos
- Asignar etiquetas a los deployment, deployment config
- Asignar Tolerations a los deployments, deployment config
