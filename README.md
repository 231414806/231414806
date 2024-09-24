> Aquí tienes un archivo  README.md  que incluye instrucciones y un ejemplo de cómo integrar un módulo JavaScript y estilos CSS en un documento HTML. El ejemplo muestra cómo usar la etiqueta  <script>  para cargar un módulo JavaScript y la etiqueta  <style>  para definir estilos en línea:
 
## Integración de Módulo JavaScript y Estilos CSS en HTML
 
Este ejemplo muestra cómo integrar un módulo JavaScript y aplicar estilos CSS en un documento HTML.
 
### Estructura del Proyecto
 
```plaintext
project-folder/
│
├── index.html
├── motion-lit.js
└── README.md
```
 
### Contenido del Archivo HTML ( index.html )
 
```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ejemplo de Módulo y CSS</title>
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      height: 100vh;
      width: 100vw;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #f0f0f0;
    }
    .container {
      text-align: center;
      padding: 20px;
      background-color: #fff;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Bienvenido</h1>
    <p>Este es un ejemplo de cómo integrar un módulo JavaScript y estilos CSS en un documento HTML.</p>
  </div>
  <script type="module" src="./motion-lit.js"></script>
</body>
</html>
```
 
### Contenido del Archivo JavaScript 
`motion-lit.js`

```js
// motion-lit.js

document.addEventListener('DOMContentLoaded', () => {
  const container = document.querySelector('.container');
  container.addEventListener('mouseover', () => {
    container.style.transform = 'scale(1.1)';
  });
  container.addEventListener('mouseout', () => {
    container.style.transform = 'scale(1)';
  });
});
```
 
#### Explicación
 
1. Estructura Básica del HTML:
 
- El archivo HTML tiene una estructura básica con una etiqueta  `<head>`  que incluye los metadatos del documento y los estilos CSS.
- Los estilos CSS dentro de la etiqueta ` <style> ` establecen el diseño básico del cuerpo `body` y de un contenedor `.container` .
2. Estilos CSS:
 
- El  body  está configurado para ocupar toda la altura y anchura de la ventana ` height: 100vh; width: 100vw; `.
- El contenedor  .container  está centrado y tiene una sombra para darle un efecto de tarjeta.
3. Módulo JavaScript:
 
- El archivo  motion-lit.js  se carga como un módulo con la etiqueta  <script type="module" src="./motion-lit.js"></script> .
- El script añade eventos  mouseover  y  mouseout  al contenedor para escalar el elemento al pasar el ratón sobre él.
 
Este ejemplo muestra cómo combinar HTML, CSS y JavaScript para crear una página web interactiva y estilizada.
 
### Ejecutar el Ejemplo
 
1. Crea una carpeta para el proyecto:
 
```bash
mkdir project-folder
cd project-folder
 
2. Crea los archivos  index.html  y  motion-lit.js :
 
- Pega el código HTML en el archivo  index.html .
- Pega el código JavaScript en el archivo  motion-lit.js .
3. Abre  index.html  en tu navegador web.
 
- Deberías ver un contenedor con un título y un párrafo.
- Al pasar el ratón sobre el contenedor, este se escalará ligeramente.
 
Notas Adicionales
 
- Integración de CSS:
 
- Puedes usar archivos CSS externos en lugar de estilos en línea.
- Para ello, crea un archivo  style.css  y agrega la siguiente línea en la etiqueta  <head>  del archivo  index.html :
html Copiar
<link rel="stylesheet" href="style.css">
 
- Módulos JavaScript:
 
- Puedes usar módulos JavaScript para organizar tu código en archivos separados.

# [Mi proyecto en Azure](https://learn.microsoft.com/es-mx/azure/azure-sql/database/logical-servers?view=azuresql&tabs=portal&source=docs) 

 # Aplicaciones/[Creación de documentos](https://github.com/3449708385/bootbase1.0.1/issues/2)/ Creación de aplicaciones de Azure/Autenticación con una Azure App/[Avalonix module builders](https://myaccount.microsoft.com/groups/299e37d6-7446-47f4-a727-3c1da64d3414) 

[User account:](https://myaccount.microsoft.com/#) 
[@notebook-t.atlassian.net](https://notebook-t.atlassian.net/wiki/spaces/IS/Overview)  

```Atom
<?xml version="1.0" encoding="UTF-8" ?>
<rss version="2.0">
  <channel>
    <title>Microsoft Learn - "azure portal"</title>
    <description>The latest updates from Microsoft Learn on "azure portal"</description>
    <link>https://learn.microsoft.com</link>
    <language>es-mx</language>
    <ttl>60</ttl>
    <pubDate>Tue, 02 Apr 2024 09:25:34 GMT</pubDate>
    <lastBuildDate>Tue, 02 Apr 2024 09:25:34 GMT</lastBuildDate>
    <item>
      <title>¿Qué es Azure Portal? - Azure portal</title>
      <description>The Azure portal is a web-based, unified console that provides an alternative to command-line tools. With the Azure portal, you can manage your Azure subscription using a graphical user interface. You can build, manage, and monitor everything from simple web apps to complex cloud deployments in the portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-portal/azure-portal-overview</link>
      <pubDate>Sun, 03 Mar 2024 12:19:00 GMT</pubDate>
    </item>
    <item>
      <title>Documentación de Azure Portal - Azure portal</title>
      <description>Azure portal documentation The Azure portal is a web-based, unified console that provides an alternative to command-line tools. You can manage your Azure subscription with the Azure portal. Build, manage, and monitor everything from simple web apps to complex cloud deployments.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-portal/</link>
      <pubDate>Mon, 29 Jan 2024 23:04:00 GMT</pubDate>
    </item>
    <item>
      <title>Enumeración de asignaciones de roles de Azure mediante Azure Portal: RBAC de Azure</title>
      <description>In the Azure portal, select All services from the Azure portal menu. Select Microsoft Entra ID and then select Users or Groups. Click the user or group you want list the role assignments for. Click Azure role assignments.</description>
      <link>https://learn.microsoft.com/es-es/azure/role-based-access-control/role-assignments-list-portal</link>
      <pubDate>Thu, 30 Nov 2023 05:35:00 GMT</pubDate>
    </item>
    <item>
      <title>Autorizar el acceso a los datos de archivo en Azure Portal</title>
      <description>When you access file data using the Azure portal, the portal makes requests to Azure Files behind the scenes. These requests can be authenticated and authorized using either your Microsoft Entra account or the storage account access key..</description>
      <link>https://learn.microsoft.com/es-es/azure/storage/files/authorize-data-operations-portal</link>
      <pubDate>Wed, 15 Nov 2023 23:20:00 GMT</pubDate>
    </item>
    <item>
      <title>Crear un panel en el Azure Portal - Azure portal</title>
      <description>Sign in to the Azure portal. From the Azure portal menu, select Dashboard. Your default view might already be set to dashboard. Select Create, then select Custom. This action opens the Tile Gallery, from which you can select tiles that display different types of information.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-portal/azure-portal-dashboards</link>
      <pubDate>Tue, 28 Nov 2023 23:15:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Uso de Azure Portal para crear una red virtual - Azure Virtual Network</title>
      <description>También puede crear una cuenta de forma gratuita. Inicio de sesión en Azure Inicie sesión en Azure Portal con su cuenta de Azure.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-network/quick-create-portal</link>
      <pubDate>Wed, 28 Feb 2024 18:04:00 GMT</pubDate>
    </item>
    <item>
      <title>Visualización de la entidad de servicio de una identidad administrada en Azure Portal - Managed identities for Azure resources</title>
      <description>Sign in to the Azure portal. In the search box, Enter Microsoft Entra ID. Under Services,  Select Microsoft Entra ID and then select Enterprise applications. Under Application Type, choose All Applications and then select Apply.</description>
      <link>https://learn.microsoft.com/es-es/entra/identity/managed-identities-azure-resources/how-to-view-managed-identity-service-principal-portal</link>
      <pubDate>Mon, 23 Oct 2023 20:21:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Creación de una instancia de Azure API Management: Portal</title>
      <description>Sign in to Azure Sign in to the Azure portal. Create a new instance From the Azure portal menu, select Create a resource. You can also select Create a resource on the Azure Home page. On the Create a resource page, select Integration &gt; API Management. On the Create API Management page, on the Basics tab, enter settings.</description>
      <link>https://learn.microsoft.com/es-es/azure/api-management/get-started-create-service-instance</link>
      <pubDate>Wed, 12 Jan 2022 12:03:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Concesión de acceso de usuario a los recursos de Azure mediante Azure Portal: Azure RBAC</title>
      <description>Sign in to Azure Sign in to the Azure portal. Create a resource group In the navigation list, click Resource groups. Click New to open the Create a resource group page. Select a subscription. For Resource group name, enter example-group or another name. Click Review + create and then click Create to create the resource group.</description>
      <link>https://learn.microsoft.com/es-es/azure/role-based-access-control/quickstart-assign-role-user-portal</link>
      <pubDate>Thu, 20 Jul 2023 11:15:00 GMT</pubDate>
    </item>
    <item>
      <title>Administración de las preferencias y la configuración de Azure Portal - Azure portal</title>
      <description>Cambie la configuración de Azure Portal, como la suscripción o el directorio predeterminados, los tiempos de espera, el modo de menú, el contraste, el tema, las notificaciones, el idioma o la región, etc..</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-portal/set-preferences</link>
      <pubDate>Sun, 03 Mar 2024 12:19:00 GMT</pubDate>
    </item>
    <item>
      <title>Permitir las direcciones URL de Azure Portal en el servidor proxy o firewall - Azure portal</title>
      <description>azure portal authentication azure portal framework account data general azure services and documentation note traffic to these endpoints uses standard tcp ports for http (80) and https (443).. azure ad urls bproxy.azurewebsites.net azure url azure portal firewall rules azure ad authentication urls aadcdn.msauth.net azure portal urls. u.s. …</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-portal/azure-portal-safelist-urls</link>
      <pubDate>Mon, 18 Sep 2023 22:12:00 GMT</pubDate>
    </item>
    <item>
      <title>Actualización de una dirección IP pública: Azure Portal</title>
      <description>Sign in to the Azure portal. In the search box at the top of the portal, enter Public IP. In the search results, select Public IP addresses. In Public IP addresses, select myBasicPublicIP or the IP address you want to upgrade. Select the upgrade banner at the top of the overview section in myBasicPublicIP.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-network/ip-services/public-ip-upgrade-portal</link>
      <pubDate>Tue, 22 Aug 2023 21:55:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: creación de un registro y una zona DNS pública: Azure Portal - Azure DNS</title>
      <description>Sign in to the Azure portal Sign in to the Azure portal with your Azure account. Create a DNS zone A DNS zone contains the DNS entries for a domain. To start hosting your domain in Azure DNS, you create a DNS zone for that domain name.</description>
      <link>https://learn.microsoft.com/es-es/azure/dns/dns-getstarted-portal</link>
      <pubDate>Tue, 21 Nov 2023 05:42:00 GMT</pubDate>
    </item>
    <item>
      <title>Captura de un seguimiento del explorador para solucionar problemas - Azure portal</title>
      <description>Sign in to the Azure portal. It's important to sign in before you start the trace so that the trace doesn't contain sensitive information related to your account. Start recording the steps you take in the portal, using Steps Recorder. In the portal, navigate to the step prior to where the issue occurs. Press F12 to launch Microsoft Edge DevTools.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-portal/capture-browser-trace</link>
      <pubDate>Tue, 31 Oct 2023 17:04:00 GMT</pubDate>
    </item>
    <item>
      <title>Administración de facturación de EA en Azure Portal - Microsoft Cost Management</title>
      <description>Inicie sesión en Azure Portal. Vaya a Administración de costos + facturación y seleccione un ámbito de facturación. Seleccione su cuenta. En el menú de la izquierda, en Configuración, seleccione Activar cuenta. En la página Activar cuenta, elija Sí, deseo continuar y seleccione Activar esta cuenta.</description>
      <link>https://learn.microsoft.com/es-es/azure/cost-management-billing/manage/direct-ea-administration</link>
      <pubDate>Mon, 11 Mar 2024 22:07:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Creación de un punto de conexión privado: Azure Portal - Azure Private Link</title>
      <description>Sign in to Azure Sign in to the Azure portal. Create a virtual network and an Azure Bastion host The following procedure creates a virtual network with a resource subnet, an Azure Bastion subnet, and a Bastion host: In the portal, search for and select Virtual networks. On the Virtual networks page, select + Create.</description>
      <link>https://learn.microsoft.com/es-es/azure/private-link/create-private-endpoint-portal</link>
      <pubDate>Wed, 28 Feb 2024 18:04:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Creación de un almacén de claves de Azure Key Vault con Azure Portal</title>
      <description>Sign in to Azure Sign in to the Azure portal. Create a vault From the Azure portal menu, or from the Home page, select Create a resource. In the Search box, enter Key Vault. From the results list, choose Key Vault. On the Key Vault section, choose Create.</description>
      <link>https://learn.microsoft.com/es-es/azure/key-vault/general/quick-create-portal</link>
      <pubDate>Thu, 20 Jul 2023 11:15:00 GMT</pubDate>
    </item>
    <item>
      <title>Administración de recursos: Azure Portal - Azure Resource Manager</title>
      <description>To open a resource by the service type: Sign in to the Azure portal. In the left pane, select the Azure service. In this case, Storage accounts. If you don't see the service listed, select All services, and then select the service type. Select the resource you want to open.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-resource-manager/management/manage-resources-portal</link>
      <pubDate>Thu, 27 Jul 2023 22:00:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Creación y modificación de circuitos ExpressRoute en Azure Portal</title>
      <description>En el menú de Azure Portal, seleccione + Crear un recurso. Busque ExpressRoute y seleccione Crear. En la página Crear ExpressRoute. Proporcione el Grupo de recursos, la Región y el Nombre del circuito. Después, seleccione Siguiente: Configuración &gt;. Setting Value Resource group Seleccione Crear nuevo.</description>
      <link>https://learn.microsoft.com/es-es/azure/expressroute/expressroute-howto-circuit-portal-resource-manager</link>
      <pubDate>Fri, 01 Mar 2024 06:28:00 GMT</pubDate>
    </item>
    <item>
      <title>Visualización de las cuentas de facturación en Azure Portal - Microsoft Cost Management</title>
      <description>Check the type of your account Sign in to the Azure portal. Search for Cost Management + Billing. If you have access to just one billing scope, select Properties from the left-hand side. The Billing account type on the properties page determines the type of your account.</description>
      <link>https://learn.microsoft.com/es-es/azure/cost-management-billing/manage/view-all-accounts</link>
      <pubDate>Tue, 23 May 2023 17:21:00 GMT</pubDate>
    </item>
    <item>
      <title>Creación de una instancia de Azure Data Factory - Azure Data Factory</title>
      <description>Go to the Azure portal data factories page. After landing on the data factories page of the Azure portal, click Create. For Resource Group, take one of the following steps: Select an existing resource group from the drop-down list. Select Create new, and enter the name of a new resource group.</description>
      <link>https://learn.microsoft.com/es-es/azure/data-factory/quickstart-create-data-factory</link>
      <pubDate>Mon, 04 Dec 2023 23:04:00 GMT</pubDate>
    </item>
    <item>
      <title>Creación de su primera función en Azure Portal</title>
      <description>From the Azure portal menu or the Home page, select Create a resource. In the New page, select Compute &gt; Function App.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-functions/functions-create-function-app-portal</link>
      <pubDate>Fri, 23 Jun 2023 22:28:00 GMT</pubDate>
    </item>
    <item>
      <title>Información general del portal para desarrolladores en Azure API Management - Azure API Management</title>
      <description>You can access it from the Azure portal interface. Customize and style the managed portal through the built-in, drag-and-drop visual editor: Use the visual editor to modify pages, media, layouts, menus, styles, or website settings.</description>
      <link>https://learn.microsoft.com/es-es/azure/api-management/api-management-howto-developer-portal</link>
      <pubDate>Wed, 15 Nov 2023 18:06:00 GMT</pubDate>
    </item>
    <item>
      <title>Creación de claves SSH en Azure Portal - Azure Virtual Machines</title>
      <description>Open the Azure portal. At the top of the page, type SSH to search. Under *Marketplace, select SSH keys. On the SSH Key page, select Create. In Resource group select Create new to create a new resource group to store your keys. Type a name for your resource group and select OK. In Region select a region to store your keys.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-machines/ssh-keys-portal</link>
      <pubDate>Tue, 26 Mar 2024 22:20:00 GMT</pubDate>
    </item>
    <item>
      <title>Crear una base de datos única - Azure SQL Database</title>
      <description>Portal Azure CLI PowerShell To create a single database in the Azure portal, this quickstart starts at the Azure SQL page. Browse to the Select SQL Deployment option page. Under SQL databases, leave Resource type set to Single database, and select Create.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-sql/database/single-database-create-quickstart</link>
      <pubDate>Mon, 11 Mar 2024 17:30:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Implementación de un clúster de Azure Kubernetes Service (AKS) mediante Azure Portal - Azure Kubernetes Service</title>
      <description>On the Azure portal home page, select Create a resource. In the Categories section, select Containers &gt; Azure Kubernetes Service (AKS). On the Basics tab, configure the following options: Under Project details: Select an Azure Subscription. Create an Azure Resource group, such as myResourceGroup.</description>
      <link>https://learn.microsoft.com/es-es/azure/aks/learn/quick-kubernetes-deploy-portal</link>
      <pubDate>Tue, 19 Mar 2024 22:06:00 GMT</pubDate>
    </item>
    <item>
      <title>Portales de seguridad y centros de administración de Microsoft</title>
      <description>portal name description link microsoft entra admin center access and administer the microsoft entra family to protect your business with decentralized identity, identity protection, governance, and more, in a multi-cloud environment entra.microsoft.com azure portal view and manage all your azure resources portal.azure.com microsoft entra admin …</description>
      <link>https://learn.microsoft.com/es-es/microsoft-365/security/defender/portals</link>
      <pubDate>Tue, 12 Dec 2023 18:46:00 GMT</pubDate>
    </item>
    <item>
      <title>Implementación y configuración de Azure Firewall mediante Azure Portal</title>
      <description>Implementación y configuración de Azure Firewall mediante Azure Portal El control del acceso de red saliente es una parte importante de un plan de seguridad de red de ámbito general. Por ejemplo, puede que quiera limitar el acceso a sitios web.</description>
      <link>https://learn.microsoft.com/es-es/azure/firewall/tutorial-firewall-deploy-portal</link>
      <pubDate>Thu, 16 Nov 2023 18:05:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido para crear y usar recursos compartidos de archivos de Azure</title>
      <description>Create an Azure file share Portal PowerShell Azure CLI To create an Azure file share: Select the storage account from your dashboard. On the storage account page, in the Data storage section, select File shares. On the menu at the top of the File shares page, select + File share. The New file share page drops down. In Name, type myshare.</description>
      <link>https://learn.microsoft.com/es-es/azure/storage/files/storage-how-to-use-files-portal</link>
      <pubDate>Tue, 10 Oct 2023 22:05:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido de Azure: Establecimiento y recuperación de un secreto de Key Vault mediante Azure Portal</title>
      <description>Inicio rápido: Establecimiento y recuperación de un secreto de Azure Key Vault mediante Azure Portal Azure Key Vault es un servicio de almacenamiento seguro de secretos en la nube. Puede almacenar de forma segura claves, contraseñas, certificados y otros secretos.</description>
      <link>https://learn.microsoft.com/es-es/azure/key-vault/secrets/quick-create-portal</link>
      <pubDate>Thu, 20 Jul 2023 11:15:00 GMT</pubDate>
    </item>
    <item>
      <title>Descripción del acceso y los permisos dentro del portal de gobernanza de Microsoft Purview</title>
      <description>Open your account in the Azure portal and select the Microsoft Purview governance portal tile on the Overview page. From there, navigate to the data map on the left menu, and then select the 'Collections' tab.</description>
      <link>https://learn.microsoft.com/es-es/purview/catalog-permissions</link>
      <pubDate>Fri, 17 Nov 2023 22:35:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Importación y publicación de la primera API en Azure API Management</title>
      <description>En Azure Portal, busque y seleccione Servicios de API Management. En la página de servicios API Management, seleccione la instancia de API Management. Importación y publicación de una API de back-end Esta sección explica cómo importar y publicar una API de back-end de Especificación OpenAPI.</description>
      <link>https://learn.microsoft.com/es-es/azure/api-management/import-and-publish</link>
      <pubDate>Thu, 29 Jun 2023 21:54:00 GMT</pubDate>
    </item>
    <item>
      <title>Solucionar problemas del agente y la extensión - Azure Backup</title>
      <description>Abra Azure Portal &gt; VM &gt; Información general &gt; y compruebe el estado de la máquina virtual para asegurarse de que esté en ejecución; y vuelva a intentar la operación de copia de seguridad.</description>
      <link>https://learn.microsoft.com/es-es/azure/backup/backup-azure-troubleshoot-vm-backup-fails-snapshot-timeout</link>
      <pubDate>Tue, 19 Mar 2024 22:06:00 GMT</pubDate>
    </item>
    <item>
      <title>Permisos en el portal de cumplimiento de Microsoft Purview</title>
      <description>Roles de Azure en el portal de cumplimiento Los roles que aparecen en la secciónRoles de identificador&gt; de Microsoft Entra de la página Permisos del portal de cumplimiento son roles Microsoft Entra.</description>
      <link>https://learn.microsoft.com/es-es/purview/purview-compliance-portal-permissions</link>
      <pubDate>Wed, 03 Jan 2024 18:58:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Creación y administración de una instancia de VPN Gateway: Azure Portal - Azure VPN Gateway</title>
      <description>Create a virtual network Create a virtual network by using the following values: Resource group: TestRG1 Name: VNet1 Region: (US) East US IPv4 address space: 10.1.0.0/16 Subnet name: FrontEnd Subnet address space: 10.1.0.0/24 Sign in to the Azure portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/vpn-gateway/tutorial-create-gateway-portal</link>
      <pubDate>Mon, 20 Nov 2023 23:07:00 GMT</pubDate>
    </item>
    <item>
      <title>Uso de plantillas de elementos de trabajo de Azure DevOps para actualizar elementos de trabajo en Azure Boards - Azure Boards</title>
      <description>Puede usar plantillas de elementos de trabajo para crear elementos de trabajo o realizar actualizaciones masivas en varios elementos de trabajo. Agregue y administre plantillas de elementos de trabajo desde el portal web o desde Visual Studio 2015 o versiones anteriores.</description>
      <link>https://learn.microsoft.com/es-es/azure/devops/boards/backlogs/work-item-template</link>
      <pubDate>Wed, 06 Dec 2023 17:14:00 GMT</pubDate>
    </item>
    <item>
      <title>Historial de implementación - Azure Resource Manager</title>
      <description>Portal PowerShell Azure CLI HTTP Select the resource group you want to examine. Select the link under Deployments. Select one of the deployments from the deployment history. A summary of the deployment is displayed, including the correlation ID. Subscription deployments You can view the history of deployments to a subscription.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-resource-manager/templates/deployment-history</link>
      <pubDate>Tue, 23 May 2023 22:09:00 GMT</pubDate>
    </item>
    <item>
      <title>Instalación de aplicaciones de trabajo desde Portal de empresa de Intune aplicación para Windows</title>
      <description>Abra la aplicación Portal de empresa en el dispositivo profesional o educativo. A continuación, inicie sesión con su cuenta profesional o educativa. Puede acceder a las aplicaciones disponibles desde los siguientes lugares de Portal de empresa: Inicio: Vaya a Inicio para ver las aplicaciones destacadas de su organización.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/user-help/install-apps-cpapp-windows</link>
      <pubDate>Wed, 01 Nov 2023 17:36:00 GMT</pubDate>
    </item>
    <item>
      <title>Aspectos básicos de Microsoft Azure AI: Computer Vision - Training</title>
      <description>prerequisites ability to navigate the azure portal save modules in this learning path fundamentals of computer vision fundamentals of facial recognition fundamentals of optical character recognition. explore computer vision in microsoft azure ai 900 ai900 azure computer vision aidemos/microsoft.com/computer-vision. custom machine learning models …</description>
      <link>https://learn.microsoft.com/es-es/training/paths/explore-computer-vision-microsoft-azure/</link>
      <pubDate>Thu, 16 Nov 2023 00:12:00 GMT</pubDate>
    </item>
    <item>
      <title>Descripción de las características y herramientas de Azure para la gobernanza y el cumplimiento - Training</title>
      <description>learning objectives describe the purpose of microsoft purview describe the purpose of azure policy describe the purpose of resource locks describe the purpose of the service trust portal save prerequisites basic familiarity with it terms and concepts introduction min describe the purpose of microsoft purview min describe the purpose of azure …</description>
      <link>https://learn.microsoft.com/es-es/training/modules/describe-features-tools-azure-for-governance-compliance/</link>
      <pubDate>Wed, 13 Mar 2024 16:55:00 GMT</pubDate>
    </item>
    <item>
      <title>Agregar y asignar la aplicación de Windows Portal de empresa para Intune dispositivos administrados - Microsoft Intune</title>
      <description>The Company Portal app will be installed in device context (also known as system-context) when assigned to the Autopilot group and will be installed on the device before the user logs in. Create and Assign the Company Portal app Sign in to the Microsoft Intune admin center with your admin account. Select Apps &gt; All apps &gt; Add.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/apps/store-apps-company-portal-autopilot</link>
      <pubDate>Tue, 27 Feb 2024 23:40:00 GMT</pubDate>
    </item>
    <item>
      <title>Obtener la aplicación Portal de empresa de Intune</title>
      <description>Open the Company Portal app on your device. Enter the email address associated with your work or school account and then tap Next. Tap Sign in with a certificate. Tap Continue to use the certificate. Wait while the app verifies your certificate. When done, you can access the features in the app and your organization's resources.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/user-help/sign-in-to-the-company-portal</link>
      <pubDate>Wed, 01 Nov 2023 17:36:00 GMT</pubDate>
    </item>
    <item>
      <title>Agregar manualmente la aplicación Portal de empresa de Windows 10 - Microsoft Intune</title>
      <description>Descarga de la aplicación de Portal de empresa sin conexión Busque y seleccione la aplicación Portal de empresa. Establezca el tipo de licenciaen Sin conexión. Las aplicaciones sin conexión se administran mediante Intune, mientras que las aplicaciones en línea las administra la tienda.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/apps/store-apps-company-portal-app</link>
      <pubDate>Tue, 14 Nov 2023 23:57:00 GMT</pubDate>
    </item>
    <item>
      <title>Inscripción de un dispositivo Android con Portal de empresa de Intune</title>
      <description>Open the Company Portal app and sign in with your work or school account. If prompted to, review notification permissions for Company Portal. You can adjust notification permissions anytime in the Settings app. If you're prompted to accept your organization's terms and conditions, tap ACCEPT ALL. Review what your organization can and can't see.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/user-help/enroll-device-android-company-portal</link>
      <pubDate>Wed, 22 Nov 2023 18:58:00 GMT</pubDate>
    </item>
    <item>
      <title>Configuración de las aplicaciones del Portal de empresa de Intune, el sitio web del Portal de empresa y la aplicación de Intune - Microsoft Intune</title>
      <description>Configuración Puede configurar la experiencia de Portal de empresa específicamente para la inscripción, privacidad, notificaciones, categorías de dispositivos, orígenes de aplicaciones y acciones de autoservicio.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/apps/company-portal-app</link>
      <pubDate>Thu, 29 Feb 2024 00:09:00 GMT</pubDate>
    </item>
    <item>
      <title>Adición de la Portal de empresa para la aplicación macOS - Microsoft Intune</title>
      <description>For personal device or manual enrollment, the Company Portal app must be downloaded and installed to initiate enrollment. See Instruct users to download and install Company Portal. Instruct users to download and install Company Portal You can instruct users to download, install, and sign in to Company Portal for macOS.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/apps/apps-company-portal-macos</link>
      <pubDate>Mon, 04 Dec 2023 10:03:00 GMT</pubDate>
    </item>
    <item>
      <title>AZ-700 Diseño e implementación de soluciones para Redes de Microsoft Azure - Training</title>
      <description>AZ-700 Diseño e implementación de soluciones para Redes de Microsoft Azure Obtenga información sobre cómo diseñar e implementar una infraestructura de red segura en Azure y cómo establecer la conectividad híbrida, el enrutamiento, el acceso privado a los servicios de Azure y la supervisión en Azure.</description>
      <link>https://learn.microsoft.com/es-es/training/paths/design-implement-microsoft-azure-networking-solutions-az-700/</link>
      <pubDate>Thu, 16 Nov 2023 00:12:00 GMT</pubDate>
    </item>
    <item>
      <title>Quitar el dispositivo de Portal de empresa de Intune para Android</title>
      <description>Sign in to Company Portal. Tap the main menu. Tap Remove Company Portal. Tap OK to remove Company Portal and unenroll the device you're on. ![ NOTE] You can temporarily disable the app without uninstalling it if you plan to use it again. After you re-enable the app you must also re-enroll your device.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/user-help/unenroll-your-device-from-intune-android</link>
      <pubDate>Wed, 12 Jul 2023 21:16:00 GMT</pubDate>
    </item>
    <item>
      <title>Portal de cumplimiento de Microsoft Purview.</title>
      <description>To access the compliance portal, go to https://compliance.microsoft.com and sign in as a global administrator, compliance administrator, or compliance data administrator. Next steps Visit Microsoft Purview Compliance Manager to see your compliance score and start managing compliance for your organization. To learn more, see Compliance Manager.</description>
      <link>https://learn.microsoft.com/es-es/purview/purview-compliance-portal</link>
      <pubDate>Wed, 03 Jan 2024 18:58:00 GMT</pubDate>
    </item>
    <item>
      <title>permisos de Microsoft Defender para Office 365 en el portal de Microsoft Defender</title>
      <description>las siguientes acciones están disponibles para email &amp; grupos de roles de colaboración en el portal de defender: creación de grupos de roles copiar grupos de roles modificación de la pertenencia a grupos de roles modificar asignaciones de roles (solo grupos de roles personalizados) quitar grupos de roles (solo grupos de roles personalizados) …</description>
      <link>https://learn.microsoft.com/es-es/microsoft-365/security/office-365-security/mdo-portal-permissions</link>
      <pubDate>Wed, 15 Nov 2023 17:18:00 GMT</pubDate>
    </item>
    <item>
      <title>Etiquetado de recursos, grupos de recursos y suscripciones para una organización lógica - Azure Resource Manager</title>
      <description>Describe las condiciones y limitaciones para usar etiquetas con recursos de Azure.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-resource-manager/management/tag-resources</link>
      <pubDate>Thu, 20 Apr 2023 22:03:00 GMT</pubDate>
    </item>
    <item>
      <title>Exportación de plantilla en Azure Portal - Azure Resource Manager</title>
      <description>Use Azure Portal para exportar una plantilla de Azure Resource Manager desde los recursos de la suscripción.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-resource-manager/templates/export-template-portal</link>
      <pubDate>Wed, 09 Aug 2023 11:19:00 GMT</pubDate>
    </item>
    <item>
      <title>Implementación de recursos con Azure Portal - Azure Resource Manager</title>
      <description>Utilice Azure Portal y Azure Resource Manager para implementar los recursos en un grupo de recursos de su suscripción.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-resource-manager/templates/deploy-portal</link>
      <pubDate>Tue, 08 Aug 2023 21:59:00 GMT</pubDate>
    </item>
    <item>
      <title>Captura de una imagen de máquina virtual con el portal - Azure Virtual Machines</title>
      <description>Cree una imagen de una máquina virtual mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-machines/capture-image-portal</link>
      <pubDate>Fri, 16 Jun 2023 21:45:00 GMT</pubDate>
    </item>
    <item>
      <title>Conexión con Azure Blob Storage mediante SFTP - Azure Storage</title>
      <description>Aprenda a habilitar la compatibilidad con SFTP para Azure Blob Storage a fin de que pueda conectarse directamente a su cuenta de Azure Storage mediante un cliente SFTP.</description>
      <link>https://learn.microsoft.com/es-es/azure/storage/blobs/secure-file-transfer-protocol-support-how-to</link>
      <pubDate>Thu, 12 Oct 2023 11:16:00 GMT</pubDate>
    </item>
    <item>
      <title>Preguntas más frecuentes sobre Azure for Students y Azure Dev Tools for Teaching</title>
      <description>Encuentre respuestas a algunas preguntas comunes sobre Azure for Students, Azure for Students Starter y Azure Dev Tools for Teaching.</description>
      <link>https://learn.microsoft.com/es-es/azure/education-hub/azure-dev-tools-teaching/program-faq</link>
      <pubDate>Tue, 21 Nov 2023 23:11:00 GMT</pubDate>
    </item>
    <item>
      <title>Habilitación del cifrado de un extremo a otro mediante el cifrado en host con discos administrados - Azure Portal - Azure Virtual Machines</title>
      <description>Use el cifrado en el host para habilitar el cifrado de un extremo a otro en los discos administrados de Azure mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-machines/disks-enable-host-based-encryption-portal</link>
      <pubDate>Wed, 15 Nov 2023 15:28:00 GMT</pubDate>
    </item>
    <item>
      <title>Incorporación a Azure Security Center para IoT</title>
      <description>https://aka.ms/iotshow/securitycommunityAzure Security Center para IoT puede ayudarle a supervisar y administrar la posición de seguridad de IoT. Las organizaciones ahora pueden proteger fácilmente sus implementaciones de IoT mediante cientos de evaluaciones de seguridad integradas extraídas de los procedimientos recomendados del sector o crear reglas personalizadas en un panel central. Con las funcionalidades de seguridad de IoT recién agregadas, ahora puede reducir la superficie expuesta a ataques para la solución de Azure IoT y corregir los problemas antes de que se puedan aprovechar.En este episodio de IoT Show, los expertos de IoT Security muestran cómo incorporarse a Azure Security Center para IoT y demostrar algunos de los muchos valores de seguridad que obtendrá.&amp;nbsp;Para más información, visite la documentación de Azure Security Center para IoT en: https://aka.ms/iot-security-docsÚnase a nuestra comunidad en: https://aka.ms/iot-security-community </description>
      <link>https://learn.microsoft.com/es-es/shows/internet-of-things-show/onboard-to-azure-security-center-for-iot</link>
      <pubDate>Fri, 15 Oct 2021 20:27:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Enrutamiento del tráfico de red con una tabla de rutas en Azure Portal</title>
      <description>En este tutorial, aprenderá a enrutar el tráfico de red con una tabla de rutas mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-network/tutorial-create-route-table-portal</link>
      <pubDate>Mon, 11 Sep 2023 21:49:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: implementación de un contenedor de Docker en una instancia de contenedor (portal) - Azure Container Instances</title>
      <description>En este inicio rápido, usará Azure Portal para implementar rápidamente una aplicación web en contenedores que se ejecuta en una instancia de contenedor aislada de Azure</description>
      <link>https://learn.microsoft.com/es-es/azure/container-instances/container-instances-quickstart-portal</link>
      <pubDate>Thu, 20 Jul 2023 11:15:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Creación de un perfil de Azure Front Door con Azure Portal</title>
      <description>En este inicio rápido se detalla cómo usar Azure Front Door Service en una aplicación web global de alta disponibilidad y rendimiento a través de Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/frontdoor/create-front-door-portal</link>
      <pubDate>Tue, 03 Oct 2023 17:17:00 GMT</pubDate>
    </item>
    <item>
      <title>Portal para desarrolladores de Teams - Teams</title>
      <description>En este artículo, aprenderá a crear una aplicación completamente nueva e importar una aplicación existente en el Portal para desarrolladores de Teams. Además, obtenga información sobre changelog for Developer Portal.</description>
      <link>https://learn.microsoft.com/es-es/microsoftteams/platform/concepts/build-and-test/teams-developer-portal</link>
      <pubDate>Wed, 23 Aug 2023 11:44:00 GMT</pubDate>
    </item>
    <item>
      <title>Documentación de Azure Resource Manager</title>
      <description>Azure Resource Manager es el servicio de implementación y administración para Azure.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-resource-manager/</link>
      <pubDate>Fri, 19 Jan 2024 12:21:00 GMT</pubDate>
    </item>
    <item>
      <title>Asignación de roles de Azure a usuarios externos mediante Azure Portal - Azure RBAC</title>
      <description>Aprenda a conceder acceso a recursos de Azure para los usuarios externos a una organización mediante Azure Portal y el control de acceso basado en rol (RBAC) de Azure.</description>
      <link>https://learn.microsoft.com/es-es/azure/role-based-access-control/role-assignments-external-users</link>
      <pubDate>Wed, 11 Oct 2023 11:19:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Hospedaje del dominio en Azure DNS</title>
      <description>En este tutorial, aprenderá a configurar Azure DNS para hospedar las zonas DNS con el Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/dns/dns-delegate-domain-azure-dns</link>
      <pubDate>Thu, 30 Nov 2023 22:58:00 GMT</pubDate>
    </item>
    <item>
      <title>Tecnologías de implementación en Azure Functions</title>
      <description>Conozca las distintas formas de implementación de código en Azure Functions.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-functions/functions-deployment-technologies</link>
      <pubDate>Wed, 25 Oct 2023 22:05:00 GMT</pubDate>
    </item>
    <item>
      <title>Búsqueda de un identificador de inquilino, un nombre de dominio y un identificador de objeto de usuario - Partner Center</title>
      <description>Obtenga información sobre cómo buscar identificadores en Azure Portal: el identificador de inquilino de Microsoft Entra de una organización, el nombre de dominio o el identificador de objeto de usuario específico. Algunas tareas necesitan esta información: área de trabajo de configuración de la cuenta.</description>
      <link>https://learn.microsoft.com/es-es/partner-center/find-ids-and-domain-names</link>
      <pubDate>Fri, 10 Nov 2023 17:02:00 GMT</pubDate>
    </item>
    <item>
      <title>Definición de atributos personalizados en Azure Active Directory B2C</title>
      <description>Defina atributos personalizados para su aplicación en Azure Active Directory B2C a fin de recopilar información sobre sus clientes.</description>
      <link>https://learn.microsoft.com/es-es/azure/active-directory-b2c/user-flow-custom-attributes</link>
      <pubDate>Tue, 21 Nov 2023 12:14:00 GMT</pubDate>
    </item>
    <item>
      <title>Requerir MFA para la administración de Azure con acceso condicional - Microsoft Entra ID</title>
      <description>Cree una directiva de acceso condicional personalizada para exigir autenticación multifactor para las tareas de administración de Azure</description>
      <link>https://learn.microsoft.com/es-es/entra/identity/conditional-access/howto-conditional-access-policy-azure-management</link>
      <pubDate>Mon, 23 Oct 2023 20:21:00 GMT</pubDate>
    </item>
    <item>
      <title>Características y extensiones de las máquinas virtuales de Azure para Windows - Azure Virtual Machines</title>
      <description>Obtenga información sobre las extensiones que están disponibles para máquinas virtuales Windows de Azure, agrupadas en función de las cosas que hacen o mejoran.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-machines/extensions/features-windows</link>
      <pubDate>Thu, 12 Oct 2023 11:16:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Conexión a un servidor SQL de Azure mediante un punto de conexión privado de Azure: Azure Portal</title>
      <description>Comience a trabajar con este tutorial para aprender a conectarse a una cuenta de almacenamiento de forma privada a través de un punto de conexión privado de Azure mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/private-link/tutorial-private-endpoint-sql-portal</link>
      <pubDate>Wed, 14 Feb 2024 23:11:00 GMT</pubDate>
    </item>
    <item>
      <title>Guía de inicio rápido de Azure: Creación de un centro de eventos mediante Azure Portal - Azure Event Hubs</title>
      <description>En este inicio rápido aprenderá a crear un centro de eventos de Azure mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/event-hubs/event-hubs-create</link>
      <pubDate>Mon, 27 Nov 2023 23:09:00 GMT</pubDate>
    </item>
    <item>
      <title>Implementación de Azure File Sync</title>
      <description>Aprenda a implementar Azure File Sync, desde el principio hasta el final, mediante Azure Portal, PowerShell o la CLI de Azure.</description>
      <link>https://learn.microsoft.com/es-es/azure/storage/file-sync/file-sync-deployment-guide</link>
      <pubDate>Fri, 29 Sep 2023 22:13:00 GMT</pubDate>
    </item>
    <item>
      <title>Comprobación del estado de cumplimiento en Portal de empresa de Intune</title>
      <description>Inicie una comprobación manual del dispositivo en Portal de empresa para actualizar el estado de la configuración del dispositivo y recuperar el acceso a los recursos profesionales o educativos.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/user-help/sync-your-device-manually-ios</link>
      <pubDate>Wed, 05 Apr 2023 23:02:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Conexión de redes virtuales con emparejamiento de VNet: Azure Portal</title>
      <description>En este tutorial, aprenderá a conectar las redes virtuales con emparejamiento de redes virtuales mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-network/tutorial-connect-virtual-networks-portal</link>
      <pubDate>Fri, 08 Sep 2023 16:47:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Creación de una instancia pública de Load Balancer: Azure Portal - Azure Load Balancer</title>
      <description>En esta guía de inicio rápido se muestra cómo crear una instancia de Load Balancer mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/load-balancer/quickstart-load-balancer-standard-public-portal</link>
      <pubDate>Tue, 24 Oct 2023 22:04:00 GMT</pubDate>
    </item>
    <item>
      <title>Uso del portal de gobernanza de Microsoft Purview</title>
      <description>En este artículo se describe cómo usar el portal de gobernanza de Microsoft Purview.</description>
      <link>https://learn.microsoft.com/es-es/purview/use-microsoft-purview-governance-portal</link>
      <pubDate>Fri, 20 Oct 2023 17:44:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Tráfico web directo mediante el portal - Azure Application Gateway</title>
      <description>En esta guía de inicio rápido, obtendrá información sobre cómo utilizar Azure Portal para crear una instancia de Azure Application Gateway que dirija el tráfico web a las máquinas virtuales de un grupo de back-end.</description>
      <link>https://learn.microsoft.com/es-es/azure/application-gateway/quick-create-portal</link>
      <pubDate>Wed, 28 Feb 2024 23:08:00 GMT</pubDate>
    </item>
    <item>
      <title>Creación de una función en Azure que se ejecuta según una programación</title>
      <description>Obtenga información sobre cómo usar Azure Portal para crear una función que se ejecuta según la programación que usted defina.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-functions/functions-create-scheduled-function</link>
      <pubDate>Mon, 27 Jun 2022 11:03:00 GMT</pubDate>
    </item>
    <item>
      <title>Descripción de las características y herramientas para administrar e implementar recursos de Azure - Training</title>
      <description>En este módulo se describen las herramientas y características que ayudan a administrar e implementar recursos en Azure.</description>
      <link>https://learn.microsoft.com/es-es/training/modules/describe-features-tools-manage-deploy-azure-resources/</link>
      <pubDate>Fri, 15 Mar 2024 17:04:00 GMT</pubDate>
    </item>
    <item>
      <title>Documentación de Azure Key Vault</title>
      <description>Aprenda a usar Key Vault para crear y mantener las claves usadas para el acceso y el cifrado de sus recursos en la nube, aplicaciones y soluciones. Tutoriales, referencias de API y mucho más.</description>
      <link>https://learn.microsoft.com/es-es/azure/key-vault/</link>
      <pubDate>Thu, 22 Feb 2024 18:06:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Incorporación de la autenticación de aplicación a una aplicación web en Azure App Service - Azure App Service</title>
      <description>En este tutorial, aprenderá a habilitar la autenticación y la autorización de aplicación para una aplicación web que se ejecuta en Azure App Service. Limite el acceso a la aplicación web solo a los usuarios de su organización.</description>
      <link>https://learn.microsoft.com/es-es/azure/app-service/scenario-secure-app-authentication-app-service</link>
      <pubDate>Tue, 19 Mar 2024 22:06:00 GMT</pubDate>
    </item>
    <item>
      <title>Actualización de la aplicación Portal de empresa</title>
      <description>Obtenga la versión más reciente de la aplicación Portal de empresa en dispositivos Android, iOS, macOS y Windows.</description>
      <link>https://learn.microsoft.com/es-es/mem/intune/user-help/install-a-new-version-of-the-company-portal-app</link>
      <pubDate>Thu, 30 Nov 2023 10:02:00 GMT</pubDate>
    </item>
    <item>
      <title>Configuración del emparejamiento de un circuito ExpressRoute: Azure Portal</title>
      <description>En esta guía se muestra cómo crear y aprovisionar emparejamientos de instancias privadas de ExpressRoute y Microsoft mediante Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/expressroute/expressroute-howto-routing-portal-resource-manager</link>
      <pubDate>Fri, 15 Sep 2023 22:12:00 GMT</pubDate>
    </item>
    <item>
      <title>Descripción de la detección y la respuesta de los puntos de conexión - Microsoft Defender for Cloud</title>
      <description>Obtenga información sobre la implementación de Microsoft Defender para punto de conexión desde Microsoft Defender for Cloud para proteger máquinas de Azure, híbridas y de varias nubes.</description>
      <link>https://learn.microsoft.com/es-es/azure/defender-for-cloud/integration-defender-for-endpoint</link>
      <pubDate>Mon, 18 Mar 2024 17:05:00 GMT</pubDate>
    </item>
    <item>
      <title>Aspectos básicos de los servicios de Azure AI - Training</title>
      <description>Este módulo es una introducción a cómo se pueden usar los servicios de Azure AI para compilar aplicaciones.</description>
      <link>https://learn.microsoft.com/es-es/training/modules/fundamentals-azure-ai-services/</link>
      <pubDate>Tue, 05 Dec 2023 18:14:00 GMT</pubDate>
    </item>
    <item>
      <title>Información general sobre la aplicación Administración de portales</title>
      <description>Aprenda a usar la aplicación de Administración de portales.</description>
      <link>https://learn.microsoft.com/es-es/power-pages/configure/portal-management-app</link>
      <pubDate>Wed, 21 Feb 2024 18:34:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Importación de un certificado en Key Vault mediante Azure Portal</title>
      <description>Tutorial que muestra cómo importar un certificado en Azure Key Vault</description>
      <link>https://learn.microsoft.com/es-es/azure/key-vault/certificates/tutorial-import-certificate</link>
      <pubDate>Mon, 16 Oct 2023 22:16:00 GMT</pubDate>
    </item>
    <item>
      <title>Inicio rápido: Creación de una zona DNS privada de Azure mediante Azure Portal</title>
      <description>En este inicio rápido se crean y se prueban una zona DNS privada y un registro en Azure DNS. Esta es una guía paso a paso para crear y administrar su primer registro y zona DNS privada con Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/dns/private-dns-getstarted-portal</link>
      <pubDate>Tue, 20 Jun 2023 11:22:00 GMT</pubDate>
    </item>
    <item>
      <title>Configurar una directiva de administración del ciclo de vida - Azure Storage</title>
      <description>Configure una directiva de administración del ciclo de vida para mover datos automáticamente entre los niveles de acceso frecuente, esporádico y de archivo durante su ciclo de vida.</description>
      <link>https://learn.microsoft.com/es-es/azure/storage/blobs/lifecycle-management-policy-configure</link>
      <pubDate>Tue, 12 Sep 2023 11:19:00 GMT</pubDate>
    </item>
    <item>
      <title>Conexión de GitHub y Azure</title>
      <description>Recursos para conectarse a GitHub desde Azure y otros servicios.</description>
      <link>https://learn.microsoft.com/es-es/azure/developer/github/connect-from-azure</link>
      <pubDate>Mon, 06 Nov 2023 17:58:00 GMT</pubDate>
    </item>
    <item>
      <title>Solución de problemas al registrarse para obtener una nueva cuenta en Azure Portal - Microsoft Cost Management</title>
      <description>Resolución de un problema al intentar suscribirse a una nueva cuenta en Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/cost-management-billing/troubleshoot-subscription/troubleshoot-azure-sign-up</link>
      <pubDate>Wed, 17 Jan 2024 23:12:00 GMT</pubDate>
    </item>
    <item>
      <title>Adición, cambio o eliminación de una subred</title>
      <description>Obtenga información sobre cómo agregar, cambiar o eliminar subredes de red virtual mediante Azure Portal, la CLI de Azure o Azure PowerShell.</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-network/virtual-network-manage-subnet</link>
      <pubDate>Wed, 15 Nov 2023 15:28:00 GMT</pubDate>
    </item>
    <item>
      <title>Uso de .NET para conectarse y consultar una base de datos en Windows, Linux o macOS - Azure SQL Database &amp; SQL Managed Instance</title>
      <description>En este artículo se muestra cómo usar .NET para crear un programa que se conecta a una base de datos de Azure SQL Database o Instancia administrada de Azure SQL y realiza consultas en ella mediante instrucciones Transact-SQL.</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-sql/database/connect-query-dotnet-core</link>
      <pubDate>Wed, 18 Oct 2023 22:42:00 GMT</pubDate>
    </item>
    <item>
      <title>Roles personalizados de Azure: RBAC de Azure</title>
      <description>Aprenda a crear roles personalizados de Azure con el control de acceso basado en roles de Azure (RBAC de Azure) para la administración de acceso específico de recursos de Azure.</description>
      <link>https://learn.microsoft.com/es-es/azure/role-based-access-control/custom-roles</link>
      <pubDate>Wed, 15 Nov 2023 18:06:00 GMT</pubDate>
    </item>
    <item>
      <title>Creación, modificación o eliminación de un grupo de seguridad de red de Azure</title>
      <description>Aprenda a crear, cambiar o eliminar un grupo de seguridad de red (NSG).</description>
      <link>https://learn.microsoft.com/es-es/azure/virtual-network/manage-network-security-group</link>
      <pubDate>Tue, 19 Mar 2024 22:06:00 GMT</pubDate>
    </item>
    <item>
      <title>Creación de un recurso compartido de archivos SMB de Azure - Azure Files</title>
      <description>Creación y eliminación de recursos compartidos de archivos SMB de Azure mediante Azure Portal, Azure PowerShell o la CLI de Azure.</description>
      <link>https://learn.microsoft.com/es-es/azure/storage/files/storage-how-to-create-file-share</link>
      <pubDate>Wed, 27 Mar 2024 22:05:00 GMT</pubDate>
    </item>
    <item>
      <title>Tutorial: Implementar Azure Bastion mediante la configuración especificada: Azure Portal</title>
      <description>Aprenda a implementar Azure Bastion mediante la configuración que especifique en Azure Portal.</description>
      <link>https://learn.microsoft.com/es-es/azure/bastion/tutorial-create-host-portal</link>
      <pubDate>Mon, 20 Nov 2023 23:07:00 GMT</pubDate>
    </item>
    <item>
      <title>Errores de registro del proveedor de recursos - Azure Resource Manager</title>
      <description>Describe cómo resolver errores de registro del proveedor de recursos para recursos implementados con un archivo Bicep o con la plantilla de Azure Resource Manager (plantilla de ARM).</description>
      <link>https://learn.microsoft.com/es-es/azure/azure-resource-manager/troubleshooting/error-register-resource-provider</link>
      <pubDate>Thu, 05 Oct 2023 11:19:00 GMT</pubDate>
    </item>
    <item>
      <title>Información general de API web de portales de Power Pages</title>
      <description>Aprenda a utilizar la API web de portales para crear, leer, actualizar y eliminar tablas de Microsoft Dataverse de las páginas de sus sitios de Power Pages.</description>
      <link>https://learn.microsoft.com/es-es/power-pages/configure/web-api-overview</link>
      <pubDate>Fri, 15 Sep 2023 18:31:00 GMT</pubDate>
    </item>
  </channel>
</rss>
```

## Generación de un JWT

Aprende a crear un JSON Web Token (JWT) para autenticarte en determinados puntos de conexión de API REST con tu Azure App.

### Sobre JSON Web Token (JWT)

Para la autenticación como una aplicación o la generación de un token de acceso de instalación, debes generar un JSON Web Token (JWT). Si un punto de conexión de la API de REST necesita un JWT, la documentación de ese punto de conexión indicará que debes usar un JWT para acceder al punto de conexión.

El JWT debe estar firmado con el algoritmo RS256 y contener las siguientes notificaciones:

- `iat`: Emitido a las. Representa la hora a la que se creó el JWT. Para protegerte contra el desfase del reloj, se recomienda establecer este valor 60 segundos en el pasado y asegurarte de que la fecha y hora del servidor se establezcan con precisión (por ejemplo, mediante el Protocolo de hora de red).
- `exp`: Expira a las. Representa la hora de expiración del JWT, después de la cual no se puede usar para solicitar un token de instalación. El valor de tiempo debe ser máximo 10 minutos después.
- `iss`: Emisor. Representa el ID de tu Azure App. Este valor se usa para buscar la clave pública correcta para comprobar la firma del JWT. Puedes encontrar el ID de la aplicación utilizando el punto de conexión de la API de REST GET /app. Para obtener más información, consulta "Aplicaciones" en la documentación de la API de REST.
- `alg`: Algoritmo de código de autenticación de mensajes. Debería ser RS256, ya que el JWT debe firmarse mediante el algoritmo RS256.

Para usar un JWT, pásalo en el encabezado Authorization de una solicitud de API. Por ejemplo:

 
``` 
curl --request GET 
--url "https://api.azure.com/app" 
--header "Accept: application/vnd.azure+json" 
--header "Authorization: Bearer YOUR_JWT" 
--header "X-Azure-Api-Version: 2022-11-28"
 ```
 

En la mayoría de los casos, puedes usar `Authorization: Bearer` o `Authorization: token` para pasar un token. Sin embargo, si vas a pasar un token web JSON (JWT), debes usar `Authorization: Bearer`.

### Generación de un JSON Web Token (JWT)

La mayoría de los lenguajes de programación tienen un paquete que puede generar un JWT. En todos los casos, debes tener una clave privada y el ID de tu Azure App. Para obtener más información sobre cómo generar una clave privada, consulta "Administración de claves privadas para aplicaciones de Azure". Puedes encontrar el ID de la aplicación utilizando el punto de conexión de la API de REST GET /app. Para obtener más información, consulta "Aplicaciones" en la documentación de la API de REST.

Nota: En vez de crear un JWT, puedes usar los SDK de Octokit de Azure para autenticarte como aplicación. El SDK se encargará de generar un JWT automáticamente y volverá a generar el JWT una vez que expire el token. Para obtener más información, consulta "Scripting con la API de REST y JavaScript".

#### Ejemplo: Uso de Ruby para generar un JWT

Nota: Debes ejecutar `gem install jwt` para instalar el paquete jwt y poder usar este script.

En el siguiente ejemplo, reemplaza `YOUR_PATH_TO_PEM` por la ruta de acceso del archivo donde se almacena la clave privada. Reemplaza `YOUR_APP_ID` por el identificador de la aplicación. Asegúrate de poner los valores `YOUR_PATH_TO_PEM` y `YOUR_APP_ID` entre comillas dobles.

```ruby
require 'openssl'
require 'jwt'  # https://rubygems.org/gems/jwt
```

# Contenido de la clave privada

```
private_pem = File.read("YOUR_PATH_TO_PEM")
private_key = OpenSSL::PKey::RSA.new(private_pem)
```

# Genera el JWT

```
payload = {
  # Tiempo de emisión, 60 segundos en el pasado para tener en cuenta el desfase del reloj
  iat: Time.now.to_i - 60,
  # Tiempo de expiración del JWT (10 minutos máximo)
  exp: Time.now.to_i + (10 * 60),
  # Identificador de la Azure App
  iss: "YOUR_APP_ID"
}

jwt = JWT.encode(payload, private_key, "RS
```

## Descripción

Este proyecto es una aplicación web desarrollada utilizando las capacidades de Microsoft Azure. 
El propósito principal de utilizar Microsoft Azure como plataforma de nube es aprovechar sus servicios y capacidades para:

1. **Alojamiento en la Nube**: Proporcionar un entorno de alojamiento en la nube escalable y confiable para aplicaciones y servicios.

2. **Desarrollo y Despliegue de Aplicaciones**: Facilitar el desarrollo, prueba y despliegue de aplicaciones y servicios en la nube.

3. **Almacenamiento de Datos**: Almacenar y gestionar datos de manera segura y eficiente en la nube.

4. **Escalabilidad**: Permitir que las aplicaciones y recursos se escalen automáticamente según la demanda, lo que garantiza un rendimiento óptimo.

5. **Seguridad y Cumplimiento**: Ofrecer herramientas y características de seguridad avanzadas y ayudar a cumplir con regulaciones y estándares de seguridad.

6. **Análisis de Datos**: Facilitar el análisis de datos mediante servicios de inteligencia empresarial y aprendizaje automático.

7. **Internet de las Cosas (IoT)**: Admitir la conectividad y la gestión de dispositivos IoT.

8. **Integración Empresarial**: Permitir la integración de sistemas y servicios empresariales.

9. **Optimización de Costos**: Ayudar a optimizar los costos de infraestructura al pagar solo por los recursos utilizados.

10. **Continuidad del Negocio**: Ofrecer opciones de recuperación ante desastres y alta disponibilidad para garantizar la continuidad del negocio.

-----------------------------------------
## Tecnologías Utilizadas
-----------------------------------------
- Azure App Service
- Azure SQL Database
- Azure Functions

-----------------------------------------
## Configuración
-----------------------------------------
Asegúrate de configurar las siguientes variables de entorno:  

`AZURE_STORAGE_CONNECTION_STRING`: 
```
DefaultEndpointsProtocol=[protocolo];AccountName=[nombre de la cuenta];AccountKey=[clave de la cuenta];EndpointSuffix=[sufijo del punto de conexión]
```
----
`AZURE_DATABASE_CONNECTION_STRING`: 
```
Server=tcp:[nombre-del-servidor].database.windows.net;Database=[nombre-de-la-base-de-datos];User ID=[nombre-de-usuario];Password=[contraseña];Trusted_Connection=False;Encrypt=True;
```

-----------------------------------------
## Instalación
-----------------------------------------

Para ejecutar este proyecto localmente, sigue estos pasos: 

1. Clona este repositorio. 
2. [Instrucciones adicionales de instalación, si las hay.] 

-----------------------------------------
## Uso
-----------------------------------------
## Describe cómo usar tu proyecto aquí.
-----------------------------------------
## Contribuciones
-----------------------------------------
Si deseas contribuir a este proyecto, sigue los pasos: 

1. Fork este repositorio. 
2. Crea una rama para tu característica (`git checkout -b caracteristica-nueva`). 
3. Realiza tus cambios y haz commit (`git commit -m 'Añade característica nueva'`). 
4. Sube tus cambios (`git push origin caracteristica-nueva`). 
5. Abre una solicitud de extracción. 

-----------------------------------------
## Créditos 
-----------------------------------------

Este proyecto ha sido posible gracias al arduo trabajo y la colaboración de diversas personas y recursos. Queremos expresar nuestro agradecimiento a:

Equipo de Desarrollo:
- [Nombre del Desarrollador 1]
- [Nombre del Desarrollador 2]
- [Nombre del Desarrollador 3]

Diseño Gráfico:
- [Nombre del Diseñador Gráfico 1]
- [Nombre del Diseñador Gráfico 2]

Colaboradores Externos:
- [Nombre del Colaborador 1]
- [Nombre del Colaborador 2]

Agradecimientos Especiales:
- [Nombre de la Persona o Entidad Especial 1]
- [Nombre de la Persona o Entidad Especial 2]

Recursos y Herramientas Utilizados:
- [Nombre de la Herramienta 1]
- [Nombre de la Herramienta 2]

Agradecemos a todos los que han contribuido de alguna manera a este proyecto, ya sea a través de su tiempo, conocimientos o recursos. Sin su apoyo, este proyecto no habría sido posible.

¡Gracias a todos por ser parte de este logro!

Carlos Alberto Ibarra Perales 

-----------------------------------------
## Licencia 
-----------------------------------------

Este proyecto está bajo la licencia Linux GNU. 

-----------------------------------------
Consulta el archivo `LICENSE`  para obtener más detalles.
-----------------------------------------
