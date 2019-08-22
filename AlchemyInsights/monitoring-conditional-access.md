---
title: Controlo de acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538774"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="4d69a-102">Controlo de acesso condicional para o Exchange</span><span class="sxs-lookup"><span data-stu-id="4d69a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="4d69a-103">Os utilizadores visados com acesso condicional irão receber uma notificação por correio electrónico se não satisfizerem os requisitos de acesso de sua organização.</span><span class="sxs-lookup"><span data-stu-id="4d69a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="4d69a-104">Para resolver, recomenda-se um ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="4d69a-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="4d69a-105">Se presume-se que o dispositivo ser inscrito, aconselhará o utilizador para ir para a aplicação de Portal da empresa e certifique-se de que é apresentada no Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="4d69a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="4d69a-106">Caso contrário, o utilizador deverá inscrever-se o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d69a-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="4d69a-107">No Azure portal Ir para **Intune \> conformidade de dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="4d69a-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="4d69a-108">No **Monitor** , clique em **cumprimento do dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="4d69a-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="4d69a-109">Ver o relatório de conformidade do dispositivo para verificar que o dispositivo do utilizador está marcado como compatível.</span><span class="sxs-lookup"><span data-stu-id="4d69a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="4d69a-110">No Azure portal Ir para **Intune \> conformidade de dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="4d69a-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="4d69a-111">Em **Gerir**, clique em **políticas**.</span><span class="sxs-lookup"><span data-stu-id="4d69a-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="4d69a-112">Na lista de políticas de conformidade, certifique-se de que é atribuído um perfil de dispositivo do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4d69a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="4d69a-113">Não se for atribuído nenhum perfil, em seguida, Intune não será possível confirmar o estado da conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d69a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="4d69a-114">Edite atribuição de acesso condicional do utilizador.</span><span class="sxs-lookup"><span data-stu-id="4d69a-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="4d69a-115">No Azure portal Ir para **Intune \> acesso condicional \> políticas**</span><span class="sxs-lookup"><span data-stu-id="4d69a-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="4d69a-116">Seleccione uma política a partir da lista</span><span class="sxs-lookup"><span data-stu-id="4d69a-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="4d69a-117">Clique em **utilizadores e grupos**</span><span class="sxs-lookup"><span data-stu-id="4d69a-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="4d69a-118">Para direccionar uma determinada política a alguém, tem de adicioná-los à lista de **inclusão** .</span><span class="sxs-lookup"><span data-stu-id="4d69a-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="4d69a-119">Para assegurar que uma pessoa for omitida da política, adicioná-los à lista de **exclusão** .</span><span class="sxs-lookup"><span data-stu-id="4d69a-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="4d69a-120">Ler mais: [como dispositivos de Monitor de acesso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="4d69a-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

