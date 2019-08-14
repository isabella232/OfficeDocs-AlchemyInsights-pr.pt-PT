---
title: Mensagens de correio electrónico de alerta 2491 da política 'Override entregues linha devido a residentes ou de utilizador'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391452"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="6680f-102">Mensagens de correio electrónico de alerta da política 'Override entregues linha devido a residentes ou de utilizador'</span><span class="sxs-lookup"><span data-stu-id="6680f-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="6680f-103">Uma alerta a política predefinida denominada "Linha entregue devido a substituição de arrendamento ou de utilizador" tiver sido efectuada a arrendatários com licenças do Office 365 ATP P1 e P2.</span><span class="sxs-lookup"><span data-stu-id="6680f-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="6680f-104">Se tiver recebido este alerta, seguem-se os passos para investigar:</span><span class="sxs-lookup"><span data-stu-id="6680f-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="6680f-105">A mensagem de alerta, clique em **Ver alerta** para ir para a página **alertas** em & o Security Center de conformidade.</span><span class="sxs-lookup"><span data-stu-id="6680f-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="6680f-106">Seleccione o alerta para vir a opção para **Ver a lista de mensagem** ou **visualizar mensagens do Explorer**.</span><span class="sxs-lookup"><span data-stu-id="6680f-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="6680f-107">Ambas as opções apresentam os detalhes da mensagem, que inclui o ID de mensagem.</span><span class="sxs-lookup"><span data-stu-id="6680f-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="6680f-108">Tenha em atenção que a ligação de ameaça Explorer automaticamente vai filtrar as mensagens que correspondam aos critérios de alertas.</span><span class="sxs-lookup"><span data-stu-id="6680f-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="6680f-109">Poderá pretender ajustar o filtro de data no Explorador de ameaça.</span><span class="sxs-lookup"><span data-stu-id="6680f-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="6680f-110">A mensagem de phishing foi entregue devido a uma substituição configurada manualmente:</span><span class="sxs-lookup"><span data-stu-id="6680f-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="6680f-111">Um permitido remetente ou domínio definidas pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="6680f-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="6680f-112">Um permitido remetente ou domínio definido pelo administrador de uma política anti-spam.</span><span class="sxs-lookup"><span data-stu-id="6680f-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="6680f-113">Um endereço IP permitido numa política de filtro de ligação.</span><span class="sxs-lookup"><span data-stu-id="6680f-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="6680f-114">Uma fluxo regra de correio (também conhecido como uma regra de transporte) que está configurada para permitir mensagens.</span><span class="sxs-lookup"><span data-stu-id="6680f-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="6680f-115">Se pensa que a mensagem foi marcada incorrectamente como phish, utilize o Outlook [suplemento de mensagem de relatório](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) para submeter amostras de mensagem para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6680f-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
