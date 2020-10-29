---
title: 2681 Simulador de ataque na Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801562"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="064d4-102">Simulador de ataque na Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="064d4-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="064d4-103">Estás a perder o Simulador de Ataque?</span><span class="sxs-lookup"><span data-stu-id="064d4-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="064d4-104">O Simulador de Ataque requer **o Microsoft Defender para o Office 365 Plan 2 (ATP Plan 2)** ou o Office **365 Enterprise E5** .</span><span class="sxs-lookup"><span data-stu-id="064d4-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="064d4-105">O Simulador de Ataque **não** está incluído no Microsoft Defender para o Office 365 Plan 1 (ATP Plan 1), no Office 365 Enterprise E3 ou em quaisquer aplicações da Microsoft 365 para subscrições empresariais.</span><span class="sxs-lookup"><span data-stu-id="064d4-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="064d4-106">A conta que utiliza para lançar ataques simulados requer permissões globais de administrador ou administrador de segurança e autenticação de vários fatores (MFA).</span><span class="sxs-lookup"><span data-stu-id="064d4-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="064d4-107">Para obter mais informações sobre os requisitos do Simulador de Ataque, consulte [este tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="064d4-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="064d4-108">Coisas importantes a saber sobre simulações de ataque de password da **Força Bruta:**</span><span class="sxs-lookup"><span data-stu-id="064d4-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="064d4-109">Se a conta-alvo tiver MFA ativada e a palavra-passe foi adivinhada corretamente, a conta não será apresentada como comprometida (o segundo fator de autenticação estará incompleto).</span><span class="sxs-lookup"><span data-stu-id="064d4-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="064d4-110">O ficheiro de senha não pode ser maior que 10 MB.</span><span class="sxs-lookup"><span data-stu-id="064d4-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="064d4-111">Use uma palavra-passe por linha e inclua uma linha em branco (retorno do transporte) após a última palavra-passe da lista.</span><span class="sxs-lookup"><span data-stu-id="064d4-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="064d4-112">Coisas importantes a saber sobre simulações de **phishing de lança:**</span><span class="sxs-lookup"><span data-stu-id="064d4-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="064d4-113">Por design, não é possível fornecer um valor personalizado para **o URL do servidor de login do Phishing.**</span><span class="sxs-lookup"><span data-stu-id="064d4-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="064d4-114">Se um destinatário utilizar [o add-in 'Ativar a mensagem's](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) reporte a mensagem como phishing, poderá não receber alertas para a mensagem (porque se trata de um ataque simulado).</span><span class="sxs-lookup"><span data-stu-id="064d4-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="064d4-115">Relatórios: Após o ataque simulado estar completo, pode clicar em **Detalhes de Ataque** para ver o relatório.</span><span class="sxs-lookup"><span data-stu-id="064d4-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="064d4-116">Para obter instruções detalhadas e novas funcionalidades no Simulador de Ataque, consulte [o Simulador de Ataque na Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="064d4-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
