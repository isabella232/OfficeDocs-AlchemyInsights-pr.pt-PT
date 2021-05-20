---
title: 2491 Alertar mensagens de e-mail da política "Phish Entregue devido a inquilino ou utilizador de override"
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544589"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="8ba25-102">Alertar mensagens de e-mail da política "Phish Entregue devido a um inquilino ou a uma override de utilizador"</span><span class="sxs-lookup"><span data-stu-id="8ba25-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="8ba25-103">Uma política de alerta predefinida denominada "Phish Entregue devido a um inquilino ou a uma override de utilizador" foi lançada para os inquilinos com o Microsoft Defender para Office 365 licenças do Office 365 P1 e P2.</span><span class="sxs-lookup"><span data-stu-id="8ba25-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="8ba25-104">Se recebeu este alerta, eis os passos para investigar:</span><span class="sxs-lookup"><span data-stu-id="8ba25-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="8ba25-105">A partir da mensagem de alerta, clique **em Ver** Alerta para ir para a **página Alertas** no Centro de conformidade & Segurança.</span><span class="sxs-lookup"><span data-stu-id="8ba25-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="8ba25-106">Selecione o alerta para ver a opção ver **a lista de mensagens** ou Ver mensagens no **Explorador.**</span><span class="sxs-lookup"><span data-stu-id="8ba25-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="8ba25-107">Ambas as opções levam-no aos detalhes da mensagem, que inclui o ID da Mensagem.</span><span class="sxs-lookup"><span data-stu-id="8ba25-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="8ba25-108">Tenha em atenção que a ligação Explorador de Ameaças irá filtrar automaticamente as mensagens que correspondem aos critérios de alerta.</span><span class="sxs-lookup"><span data-stu-id="8ba25-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="8ba25-109">Poderá ter de ajustar o filtro de datas no Explorador de Ameaças.</span><span class="sxs-lookup"><span data-stu-id="8ba25-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="8ba25-110">A mensagem de phishing foi entregue devido a uma override configurada manualmente:</span><span class="sxs-lookup"><span data-stu-id="8ba25-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="8ba25-111">Um remetente ou domínio permitido definido pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="8ba25-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="8ba25-112">Um remetente ou domínio permitido definido pelo administrador numa política antisspam.</span><span class="sxs-lookup"><span data-stu-id="8ba25-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="8ba25-113">Um endereço IP permitido numa política de filtro de ligação.</span><span class="sxs-lookup"><span data-stu-id="8ba25-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="8ba25-114">Uma regra de fluxo de correio (também conhecida como regra de transporte) que está configurada para permitir mensagens.</span><span class="sxs-lookup"><span data-stu-id="8ba25-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="8ba25-115">Se acredita que a mensagem foi marcada incorretamente como phish, utilize o [Outlook-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Report Message (Mensagem de Relatório) para submeter exemplos de mensagens à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8ba25-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
