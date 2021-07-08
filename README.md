# ex280-Final-Study-Guide

Partiendo del principio de que este examen esta orientado a administradores y no a desarrolladores, me centrare en organizarlo segun este punto de vista.

Administracion de la plataforma
- Agregar Htpasswd Identity Manager
- Administracion de Usuarios y Permisos
	- Agregar usuarios
		- Asignar cluster-admin a un usuario para dejar de usar kubeadmin
	- Crear grupos
		- Asignar permisos para creacion de projectos
		- Quitar al resto los permisos para crear proyectos
		- Asignar permisos de edicion para los desarrolladores
		- Asignar permisis de vista para los testers
- Configuracion de plantilla para proyectos
	- Agregar Network Policies
	- Agregar LimitRanges
	- Agregar Quotas
- Configurar Regiones y Zonas para el Scheduling
	- Etiquetar Nodos
	- Establecer Tains si son necesarios

Manejo de Projectos
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
