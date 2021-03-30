---
title: Obtenha uma lista de Aplicações empresariais
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405516"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="b862c-102">Obtenha uma lista de Aplicações empresariais</span><span class="sxs-lookup"><span data-stu-id="b862c-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="b862c-103">Para **obter uma lista de aplicações empresariais** (todas as aplicações ou filtradas pelo nome display, ID, Identifier URIs, etc.) através do comando Powershell, consulte [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="b862c-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="b862c-104">Para obter uma lista de objetos principais de serviço (todos os objetos ou filtrados por ID) através do comando Powershell, consulte [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="b862c-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="b862c-105">Se quiser **obter uma lista de aplicações configuradas pela SAML, seguir scripts PowerShell** pode ajudá-lo:</span><span class="sxs-lookup"><span data-stu-id="b862c-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="b862c-106">Cada Aplicação seja uma aplicação OAuth ou uma aplicação SAML (tanto de galeria como de aplicações não-galeria) teriam dois objetos criados no AAD quando o seu registo acontecesse.</span><span class="sxs-lookup"><span data-stu-id="b862c-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="b862c-107">Um é chamado de Objeto de Aplicação e o outro é o objeto principal de serviço.</span><span class="sxs-lookup"><span data-stu-id="b862c-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="b862c-108">Quando despeja as propriedades de um Objeto Principal de Serviço usando o PowerShell, descobriria que cada aplicação tem um certo número de Tags associadas a ele como:</span><span class="sxs-lookup"><span data-stu-id="b862c-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="b862c-109">As aplicações OAuth teriam uma etiqueta chamada "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="b862c-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="b862c-110">A Gallery SAML Apps teria uma etiqueta chamada "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="b862c-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="b862c-111">Não Galeria SAML Apps teria uma etiqueta chamada "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="b862c-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="b862c-112">Assim, você pode usar estas tags e descobrir que tipo de app é.</span><span class="sxs-lookup"><span data-stu-id="b862c-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="b862c-113">A tag "**WindowsAzureActiveDirectoryIntegratedApp**" é comum a todos os tipos de aplicações.</span><span class="sxs-lookup"><span data-stu-id="b862c-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="b862c-114">Você pode usar o corte seguinte para listar todas as aplicações SAML (tanto galeria como não-galeria):</span><span class="sxs-lookup"><span data-stu-id="b862c-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="b862c-115">Para obter mais informações, consulte [identificar aplicações ativadas pela SAML em Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="b862c-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="b862c-116">**Localizar e listar apenas aplicações Web**: Use o comando abaixo para obter todas as aplicações AD Azure com o tipo de aplicação "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="b862c-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="b862c-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="b862c-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="b862c-118">**Encontre e liste apenas aplicações nativas**: Executar o seguinte comando para obter todas as aplicações do cliente nativo (desktop/dispositivo móvel).</span><span class="sxs-lookup"><span data-stu-id="b862c-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="b862c-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="b862c-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="b862c-120">**Exportar todos os detalhes da aplicação Azure AD registados para o CSV**: O comando abaixo exporta todas as aplicações AD AZure com detalhes necessários para o ficheiro CSV:</span><span class="sxs-lookup"><span data-stu-id="b862c-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="b862c-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient,AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="b862c-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="b862c-122">Export-Csv "C:\AzureADApps.csv" - NoTypeInformation -Codificação UTF8</span><span class="sxs-lookup"><span data-stu-id="b862c-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="b862c-123">**Necessidade de exportar uma lista de aplicações Azure não usused** – Relatório de auditoria</span><span class="sxs-lookup"><span data-stu-id="b862c-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="b862c-124">O Azure AD pode apresentar registos de candidaturas por apenas 30 dias desde que tenha licença Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="b862c-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="b862c-125">Tem duas opções para reter os dados por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="b862c-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="b862c-126">Pode utilizar as [APIs de relato de Ad Azure](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) para recuperar os dados programáticamente e armazená-los numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="b862c-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="b862c-127">Em alternativa, pode integrar registos de auditoria num sistema SIEM de terceiros.</span><span class="sxs-lookup"><span data-stu-id="b862c-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="b862c-128">Também pode descarregar a lista de aplicações para todas as aplicações e aplicações de propriedade sob o diretório Azure Ative>Registos de Aplicações>Descarregar>todas as aplicações/aplicações próprias.</span><span class="sxs-lookup"><span data-stu-id="b862c-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="b862c-129">Para obter uma lista de aplicações através do MS Graph, consulte [as aplicações List - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) e [tipo de recurso de aplicação - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="b862c-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
