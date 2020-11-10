---
title: Erro de login oneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982542"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="feffd-102">Erro de login oneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="feffd-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="feffd-103">Se receber um erro "AADSTS50011: O URL de resposta especificado no pedido não corresponde à resposta" ao assinar na aplicação OneDrive, verifique o seguinte:</span><span class="sxs-lookup"><span data-stu-id="feffd-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="feffd-104">A sua versão OneDrive tem de ser igual ou superior à versão 20.052.XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="feffd-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="feffd-105">Para verificar a sua versão, clique no ícone OneDrive azul na área de notificação, selecione **'Definições &' > Definições > Sobre**.</span><span class="sxs-lookup"><span data-stu-id="feffd-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="feffd-106">A sua rede pode bloquear o tráfego para **g.live.com** e **oneclient.sfx.ms**.</span><span class="sxs-lookup"><span data-stu-id="feffd-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="feffd-107">Se o tráfego estiver bloqueado, o OneDrive não pode atualizar-se sozinho.</span><span class="sxs-lookup"><span data-stu-id="feffd-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="feffd-108">Trabalhe com o seu administrador de rede para garantir que tem acesso a esses URLs.</span><span class="sxs-lookup"><span data-stu-id="feffd-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="feffd-109">[Estes pontos finais](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) devem ser alcançáveis para os clientes que usam os planos da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="feffd-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="feffd-110">Se precisar de obter manualmente uma versão atual do OneDrive, visite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="feffd-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
