---
title: Acesso Condicional de Monitorização
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702914"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="ec758-102">Monitorização do Acesso Condicional para Troca</span><span class="sxs-lookup"><span data-stu-id="ec758-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="ec758-103">Os utilizadores direcionados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="ec758-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="ec758-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="ec758-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="ec758-105">Caso se presuma que o dispositivo esteja matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e verificar se aparece no Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="ec758-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="ec758-106">Se não o fizer, o utilizador deverá inscrever o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec758-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="ec758-107">No portal Azure aceda à \*\* \> conformidade do Dispositivo Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="ec758-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="ec758-108">No **Monitor** clique **na conformidade do dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="ec758-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="ec758-109">Consulte o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme.</span><span class="sxs-lookup"><span data-stu-id="ec758-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="ec758-110">No portal Azure aceda à \*\* \> conformidade do Dispositivo Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="ec758-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="ec758-111">Em **Gestão**, clique em **Políticas**.</span><span class="sxs-lookup"><span data-stu-id="ec758-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="ec758-112">Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do seu utilizador.</span><span class="sxs-lookup"><span data-stu-id="ec758-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="ec758-113">Se não for atribuído nenhum perfil, o Intune não poderá confirmar o estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec758-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="ec758-114">Editar a atribuição de acesso condicional do utilizador.</span><span class="sxs-lookup"><span data-stu-id="ec758-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="ec758-115">No portal Azure vai para Políticas de \*\* \> Acesso Condicionado \> Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="ec758-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="ec758-116">Selecione uma política da lista</span><span class="sxs-lookup"><span data-stu-id="ec758-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="ec758-117">Clique em **Utilizadores e grupos**</span><span class="sxs-lookup"><span data-stu-id="ec758-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="ec758-118">Para direcionar uma determinada política a alguém, adicione-a à lista **de incluir.**</span><span class="sxs-lookup"><span data-stu-id="ec758-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="ec758-119">Para garantir que uma pessoa é omitida da apólice, adicione-a à lista **de exclusão.**</span><span class="sxs-lookup"><span data-stu-id="ec758-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="ec758-120">Leia mais: [Como monitorizar dispositivos de acesso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="ec758-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

