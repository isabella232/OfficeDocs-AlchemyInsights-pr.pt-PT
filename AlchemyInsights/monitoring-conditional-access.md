---
title: Controlo de acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483617"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="87f91-102">Controlo de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="87f91-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="87f91-p101">Os utilizadores visados com acesso condicional irão receber uma notificação por correio electrónico se não satisfizerem os requisitos de acesso de sua organização. Para resolver, recomenda-se um ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="87f91-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="87f91-p102">Se presume-se que o dispositivo ser inscrito, aconselhará o utilizador para ir para a aplicação de Portal da empresa e certifique-se de que é apresentada no Portal da empresa. Caso contrário, o utilizador deverá inscrever-se o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f91-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="87f91-p103">No Azure portal Ir para **Intune \> conformidade de dispositivo**. No **Monitor** , clique em **cumprimento do dispositivo**. Ver o relatório de conformidade do dispositivo para verificar que o dispositivo do utilizador está marcado como compatível.</span><span class="sxs-lookup"><span data-stu-id="87f91-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="87f91-p104">No Azure portal Ir para **Intune \> conformidade de dispositivo**. Em **Gerir**, clique em **políticas**. Na lista de políticas de conformidade, certifique-se de que é atribuído um perfil de dispositivo do utilizador. Não se for atribuído nenhum perfil, em seguida, Intune não será possível confirmar o estado da conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f91-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="87f91-114">Edite atribuição de acesso condicional do utilizador.</span><span class="sxs-lookup"><span data-stu-id="87f91-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="87f91-115">No Azure portal Ir para **Intune \> acesso condicional \> políticas**</span><span class="sxs-lookup"><span data-stu-id="87f91-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="87f91-116">Seleccione uma política a partir da lista</span><span class="sxs-lookup"><span data-stu-id="87f91-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="87f91-117">Clique em **utilizadores e grupos**</span><span class="sxs-lookup"><span data-stu-id="87f91-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="87f91-p105">Para direccionar uma determinada política a alguém, tem de adicioná-los à lista de **inclusão** . Para assegurar que uma pessoa for omitida da política, adicioná-los à lista de **exclusão** .</span><span class="sxs-lookup"><span data-stu-id="87f91-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="87f91-120">Ler mais: [como dispositivos de Monitor de acesso condicional](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="87f91-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

