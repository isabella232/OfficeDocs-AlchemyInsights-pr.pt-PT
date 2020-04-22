---
title: Monitorização do Acesso Condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713729"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="2fb8a-102">Monitorização do Acesso Condicional para Troca</span><span class="sxs-lookup"><span data-stu-id="2fb8a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="2fb8a-103">Os utilizadores visados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="2fb8a-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="2fb8a-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="2fb8a-105">Se o dispositivo for presumivelmente matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e a verificar se aparece no Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="2fb8a-106">Se não o fizer, o utilizador deve inscrever o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="2fb8a-107">No portal Azure vá à \*\*conformidade do Dispositivo Intune. \> \*\*</span><span class="sxs-lookup"><span data-stu-id="2fb8a-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2fb8a-108">Sob **o monitor** clique cumprimento do **dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="2fb8a-109">Consulte o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="2fb8a-110">No portal Azure vá à \*\*conformidade do Dispositivo Intune. \> \*\*</span><span class="sxs-lookup"><span data-stu-id="2fb8a-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2fb8a-111">Em **'Gerir',** clique em **Políticas**.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="2fb8a-112">Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="2fb8a-113">Se nenhum perfil for atribuído, então intune não será capaz de confirmar o estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="2fb8a-114">Editar a atribuição de acesso condicional do utilizador.</span><span class="sxs-lookup"><span data-stu-id="2fb8a-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="2fb8a-115">No portal Azure aceda a **Intune \> Políticas de acesso \> Condicional**</span><span class="sxs-lookup"><span data-stu-id="2fb8a-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="2fb8a-116">Selecione uma política da lista</span><span class="sxs-lookup"><span data-stu-id="2fb8a-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="2fb8a-117">Clique em **Utilizadores e grupos**</span><span class="sxs-lookup"><span data-stu-id="2fb8a-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="2fb8a-118">Para direcionar uma certa política para alguém, adicione-os à lista **de Incluir.**</span><span class="sxs-lookup"><span data-stu-id="2fb8a-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="2fb8a-119">Para garantir que uma pessoa seja omitida da política, adicione-a à lista **de Excluir.**</span><span class="sxs-lookup"><span data-stu-id="2fb8a-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="2fb8a-120">Leia mais: [Como monitorizar dispositivos](https://docs.microsoft.com/intune/conditional-access-exchange-monitor) de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="2fb8a-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

