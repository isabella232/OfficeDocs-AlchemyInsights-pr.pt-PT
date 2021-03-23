---
title: Configure ponto de ligação de serviço (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037285"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="aa041-102">Configure ponto de ligação de serviço (SCP)</span><span class="sxs-lookup"><span data-stu-id="aa041-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="aa041-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="aa041-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="aa041-104">**Razão**: Incapaz de ler o objeto SCP e obter a informação do inquilino da AD AZure</span><span class="sxs-lookup"><span data-stu-id="aa041-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="aa041-105">**Resolução**: Consulte a secção [Configurar um Ponto de Ligação de Serviço](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="aa041-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="aa041-106">**Plano de ação**</span><span class="sxs-lookup"><span data-stu-id="aa041-106">**Action plan**</span></span>

- <span data-ttu-id="aa041-107">Verifique se o dispositivo recebeu o GPO para a validação controlada.</span><span class="sxs-lookup"><span data-stu-id="aa041-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="aa041-108">Certifique-se de que o GPO criou as chaves de registo.</span><span class="sxs-lookup"><span data-stu-id="aa041-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="aa041-109">Certifique-se de que tem 2 teclas criadas com o seu ID do Diretório e o domínio onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="aa041-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="aa041-110">**Configurar a definição de registo do lado do cliente para o SCP**</span><span class="sxs-lookup"><span data-stu-id="aa041-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="aa041-111">Utilize o exemplo seguinte para criar um Objeto de Política de Grupo (GPO) para implementar uma definição de registo que configura uma entrada SCP no registo dos seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="aa041-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="aa041-112">Abra uma consola de Gestão de Políticas de Grupo e crie um novo GPO no seu domínio.</span><span class="sxs-lookup"><span data-stu-id="aa041-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="aa041-113">Forneça ao seu gpo recém-criado um nome (por exemplo, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="aa041-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="aa041-114">Editar o GPO e localizar o seguinte caminho: **Configuração do computador > Preferências > Definições do Windows > Registo**.</span><span class="sxs-lookup"><span data-stu-id="aa041-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="aa041-115">Clique com o botão direito no **Registo** e selecione **New > Registry Item**.</span><span class="sxs-lookup"><span data-stu-id="aa041-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="aa041-116">No separador **Geral,** configure o seguinte:</span><span class="sxs-lookup"><span data-stu-id="aa041-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="aa041-117">**Ação**: Atualização</span><span class="sxs-lookup"><span data-stu-id="aa041-117">**Action**: Update</span></span>
    
- <span data-ttu-id="aa041-118">**Colmeia**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="aa041-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="aa041-119">**Caminho chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="aa041-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="aa041-120">**Nome de valor**: TenantId</span><span class="sxs-lookup"><span data-stu-id="aa041-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="aa041-121">**Tipo de valor**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="aa041-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="aa041-122">**Dados de valor**: O ID GUID ou Diretório da sua instância AD Azure (Este valor pode ser encontrado no **portal Azure > Azure Ative Directy > Properties > Diretório ID)**</span><span class="sxs-lookup"><span data-stu-id="aa041-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="aa041-123">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa041-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="aa041-124">Clique com o botão direito no **Registo** e selecione **New > Registry Item**.</span><span class="sxs-lookup"><span data-stu-id="aa041-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="aa041-125">No separador **Geral,** configure o seguinte:</span><span class="sxs-lookup"><span data-stu-id="aa041-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="aa041-126">**Ação**: Atualização</span><span class="sxs-lookup"><span data-stu-id="aa041-126">**Action**: Update</span></span>
    
- <span data-ttu-id="aa041-127">**Colmeia**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="aa041-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="aa041-128">**Caminho chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="aa041-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="aa041-129">**Nome de valor**: Nome do Inquilino</span><span class="sxs-lookup"><span data-stu-id="aa041-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="aa041-130">**Tipo de valor**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="aa041-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="aa041-131">**Dados de valor**: O seu nome de domínio verificado se estiver a utilizar ambientes federados, como AD FS.</span><span class="sxs-lookup"><span data-stu-id="aa041-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="aa041-132">O seu nome de domínio verificado ou o seu nome de domínio onmicrosoft.com (por exemplo, contoso.onmicrosoft).com se estiver a utilizar ambiente gerido</span><span class="sxs-lookup"><span data-stu-id="aa041-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="aa041-133">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa041-133">Click **OK**.</span></span>

7. <span data-ttu-id="aa041-134">Feche o editor para o recém-criado GPO.</span><span class="sxs-lookup"><span data-stu-id="aa041-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="aa041-135">Ligue o GPO recém-criado ao or desejado contendo computadores ligados ao domínio que pertencem à sua população de implantação controlada.</span><span class="sxs-lookup"><span data-stu-id="aa041-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="aa041-136">Para mais informações, consulte [a validação controlada da ad híbrida Azure - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) e  [Troubleshoot híbrido Azure Ative Directory juntou dispositivos | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="aa041-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









