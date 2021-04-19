---
title: Os seus utilizadores receberam e-mail malicioso
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815257"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="ac30f-102">Os seus utilizadores receberam e-mail malicioso?</span><span class="sxs-lookup"><span data-stu-id="ac30f-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="ac30f-103">Agora pode comunicar o e-mail malicioso à Microsoft através das [submissões de administrador no Centro de Conformidade e Segurança](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="ac30f-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="ac30f-104">As mensagens que são enviadas nas [submissões de administrador](https://sip.protection.office.com/reportsubmission) são digitalizadas e os seguintes resultados são apresentados na lista de opções de **detalhes**:</span><span class="sxs-lookup"><span data-stu-id="ac30f-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="ac30f-105">Caso tenha ocorrido uma falha na autenticação de e-mail do remetente no momento da entrega.</span><span class="sxs-lookup"><span data-stu-id="ac30f-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="ac30f-106">Informações sobre quaisquer ocorrências de política que possam ter afetado ou substituído o veredito de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ac30f-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="ac30f-107">Resultados da detonação atual para ver se os URLs ou os ficheiros contidos na mensagem eram mal-intencionados ou não.</span><span class="sxs-lookup"><span data-stu-id="ac30f-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="ac30f-108">Feedback das suas notas</span><span class="sxs-lookup"><span data-stu-id="ac30f-108">Feedback from graders</span></span>

<span data-ttu-id="ac30f-109">Se tiver sido encontrada uma substituição, a nova análise deve ser concluída em vários minutos.</span><span class="sxs-lookup"><span data-stu-id="ac30f-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="ac30f-110">Se não existir um problema na autenticação de e-mail ou se a entrega não tiver sido afetada por uma substituição, o feedback das suas notas poderá demorar até um dia.</span><span class="sxs-lookup"><span data-stu-id="ac30f-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="ac30f-111">Se discordar do veredito final de uma mensagem, URL ou ficheiro (bloqueado vs. não bloqueado), envie a mensagem novamente após um dia para digitalizar novamente.</span><span class="sxs-lookup"><span data-stu-id="ac30f-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="ac30f-112">Existe uma elevada probabilidade de o veredito ser alterado após submeter a mensagem novamente.</span><span class="sxs-lookup"><span data-stu-id="ac30f-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="ac30f-113">Entretanto, pode remover o e-mail malicioso das caixas de entrada dos utilizadores, seguindo as instruções descritas [neste artigo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="ac30f-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="ac30f-114">Os clientes com o Microsoft Defender para Office 365 podem:</span><span class="sxs-lookup"><span data-stu-id="ac30f-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="ac30f-115">utilizar [o explorador de ameaças para localizar e eliminar e-mails suspeitos](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="ac30f-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="ac30f-116">[utilizar ligações seguras para bloquear o acesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a um URL malicioso</span><span class="sxs-lookup"><span data-stu-id="ac30f-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="ac30f-117">monitorizar os utilizadores que clicarem e acederem a URLs maliciosos: [ver o URL de phishing e clicar em veredito de dados](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="ac30f-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="ac30f-118">iniciar [manualmente uma investigação automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="ac30f-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="ac30f-119">Também se pode proteger contra ficheiros e URLs maliciosos seguindo as instruções em [Proteção de URLs e ficheiros maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="ac30f-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>