---
title: Reencaminhar e-mails através do Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ffdaca1ba45a6f273809dbe50a7c40e8610193e1
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666527"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="8be56-102">Configurar uma aplicação ou dispositivo multifunções para enviar e-mails através do Office 365</span><span class="sxs-lookup"><span data-stu-id="8be56-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="8be56-103">Para obter mais informações sobre os passos e opções disponíveis, consulte [Como configurar uma aplicação ou dispositivo multifunções para enviar e-mails com o Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span><span class="sxs-lookup"><span data-stu-id="8be56-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="8be56-104">**Nota:** se tiver um dispositivo ou aplicação que deixou de funcionar há pouco tempo, tenha em atenção que começámos recentemente a [desativar a cifra 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption), tal como planeado.</span><span class="sxs-lookup"><span data-stu-id="8be56-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="8be56-105">Para ver os dispositivos afetados, aceda ao [relatório dos Clientes de Autenticação de SMTP](https://protection.office.com/mailflow/dashboard)</span><span class="sxs-lookup"><span data-stu-id="8be56-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="8be56-106">Os erros comuns poderão ser semelhantes a: erro/falha de Autenticação, erro/falha de TLS, erro de algoritmo de Encriptação, Algoritmo incompatível ou perda de Ligação.</span><span class="sxs-lookup"><span data-stu-id="8be56-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="8be56-107">Como resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="8be56-107">To resolve the issue:</span></span>
 - <span data-ttu-id="8be56-108">**O IIS SMTP do Windows Server 2003 deixará de funcionar – é necessária uma versão mais recente do Windows.**</span><span class="sxs-lookup"><span data-stu-id="8be56-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="8be56-109">Contacte o fornecedor do seu dispositivo ou aplicação para saber se existem cifras modernas suportadas ou atualizações.</span><span class="sxs-lookup"><span data-stu-id="8be56-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
