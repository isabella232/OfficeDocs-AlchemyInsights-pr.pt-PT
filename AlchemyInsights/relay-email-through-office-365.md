---
title: Reencaminhamento de e-mail através do Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117994"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="e8af8-102">Configurar uma aplicação ou dispositivo multifunções para enviar e-mails</span><span class="sxs-lookup"><span data-stu-id="e8af8-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="e8af8-103">Para obter mais informações sobre os passos e opções disponíveis, consulte [Como configurar uma aplicação ou dispositivo multifunções para enviar e-mails com o Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="e8af8-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="e8af8-104">Se tiver um dispositivo ou aplicação que deixou de funcionar recentemente, os problemas mais comuns são:</span><span class="sxs-lookup"><span data-stu-id="e8af8-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="e8af8-105">**Erros relacionados com a autenticação ao utilizar a submissão de cliente SMTP Auth** Recentemente, fizemos algumas alterações relacionadas com o funcionamento da Autenticação SMTP.</span><span class="sxs-lookup"><span data-stu-id="e8af8-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="e8af8-106">Para obter mais informações sobre como resolver problemas, consulte a secção de autenticação sem sucesso da secção Corrigir problemas com impressoras, [scanners](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)e aplicações LOB que enviam e-mails através de Microsoft 365 ou Office 365.</span><span class="sxs-lookup"><span data-stu-id="e8af8-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="e8af8-107">**Aceitamos apenas a versão TLS 1.2 ao criar uma ligação segura ao Office 365** Se estiver a utilizar Uma Ligação Segura (TLS), certifique-se de que o seu dispositivo de aplicação suporta TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="e8af8-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="e8af8-108">Para obter mais informações, [consulte Preparar para o TLS 1.2 no Office 365 e Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="e8af8-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="e8af8-109">Para outros problemas e soluções, consulte Corrigir problemas com impressoras, [scanners](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)e aplicações LOB que enviam e-mails através Microsoft 365 ou Office 365.</span><span class="sxs-lookup"><span data-stu-id="e8af8-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="e8af8-110">Para ver os dispositivos afetados, aceda ao [relatório dos Clientes de Autenticação de SMTP](https://protection.office.com/mailflow/dashboard)</span><span class="sxs-lookup"><span data-stu-id="e8af8-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="e8af8-111">**Nota:** Exchange Online não acomoda cenários de correio em massa.</span><span class="sxs-lookup"><span data-stu-id="e8af8-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="e8af8-112">Para enviar e-mails comerciais em massa (por exemplo, newsletters de clientes), deve utilizar fornecedores de terceiros especializados nestes serviços.</span><span class="sxs-lookup"><span data-stu-id="e8af8-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
