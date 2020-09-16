---
title: 2491 Alerte as mensagens de correio da política "Phish Delivered devido à política de inquilina ou substituição de utilizador"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728622"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="4ac34-102">Alerte as mensagens de correio da política "Phish Delivered devido à política de inquilina ou substituição de utilizador"</span><span class="sxs-lookup"><span data-stu-id="4ac34-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="4ac34-103">Uma política de alerta padrão denominada "Phish Delivered devido a inquilina ou substituição de utilizador" foi lançada para inquilinos com licenças Do Office 365 ATP P1 e P2.</span><span class="sxs-lookup"><span data-stu-id="4ac34-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="4ac34-104">Se recebeu este alerta, aqui estão os passos para investigar:</span><span class="sxs-lookup"><span data-stu-id="4ac34-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="4ac34-105">A partir da mensagem de alerta, clique em **Ver Alerta** para ir à página **Alertas** no Centro de Conformidade & de Segurança.</span><span class="sxs-lookup"><span data-stu-id="4ac34-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="4ac34-106">Selecione o alerta para ver a opção de visualizar a **lista de mensagens** ou **ver mensagens no Explorer**.</span><span class="sxs-lookup"><span data-stu-id="4ac34-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="4ac34-107">Ambas as opções levam-no aos detalhes da mensagem, que inclui o ID da mensagem.</span><span class="sxs-lookup"><span data-stu-id="4ac34-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="4ac34-108">Note que a ligação Exploradora de Ameaças filtrará automaticamente as mensagens que correspondem aos critérios de alerta.</span><span class="sxs-lookup"><span data-stu-id="4ac34-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="4ac34-109">Pode ser necessário ajustar o filtro de datas no Explorador de Ameaças.</span><span class="sxs-lookup"><span data-stu-id="4ac34-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="4ac34-110">A mensagem de phishing foi entregue devido a uma sobreposição configurada manualmente:</span><span class="sxs-lookup"><span data-stu-id="4ac34-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="4ac34-111">Um remetente ou domínio permitido definido pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ac34-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="4ac34-112">Um remetente ou domínio permitido definido pelo administrador numa política anti-correio publicitário não-correio eletrónico.</span><span class="sxs-lookup"><span data-stu-id="4ac34-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="4ac34-113">Um endereço IP permitido numa política de filtro de ligação.</span><span class="sxs-lookup"><span data-stu-id="4ac34-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="4ac34-114">Uma regra de fluxo de correio (também conhecida como regra de transporte) que está configurada para permitir a entrada de mensagens.</span><span class="sxs-lookup"><span data-stu-id="4ac34-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="4ac34-115">Se acredita que a mensagem foi incorretamente marcada como phish, utilize o [add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) da Mensagem do Relatório do Outlook para enviar amostras de mensagens à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4ac34-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
