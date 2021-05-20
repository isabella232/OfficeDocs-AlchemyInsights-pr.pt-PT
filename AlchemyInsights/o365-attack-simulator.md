---
title: Simulador de Ataque 2681 no Microsoft 365
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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545737"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="f3a0f-102">Simulador de Ataque no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f3a0f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="f3a0f-103">Não tem o Simulador de Ataque?</span><span class="sxs-lookup"><span data-stu-id="f3a0f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="f3a0f-104">O Simulador de **Ataque necessita do Microsoft Defender Office 365 Plano 2** ou Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="f3a0f-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="f3a0f-105">O Simulador de **Ataque não** está incluído no Microsoft Defender para Office 365 Plano 1, Office 365 Enterprise E3 ou Microsoft 365 Apps para Pequenas e Médias Empresas subscrições.</span><span class="sxs-lookup"><span data-stu-id="f3a0f-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="f3a0f-106">A conta que utiliza para iniciar ataques simulados requer permissões de administrador global ou administrador de segurança e a autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="f3a0f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="f3a0f-107">Para obter mais informações sobre os requisitos do Simulador de Ataque, [consulte este tópico.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="f3a0f-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="f3a0f-108">As coisas importantes a saber sobre **simulações de ataque de Forçar Palavra-passe Brute:**</span><span class="sxs-lookup"><span data-stu-id="f3a0f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="f3a0f-109">Se a conta de destino tiver a autenticação mfa ativada e a palavra-passe tiver sido corretamente adivinhar, a conta não será mostrada como comprometida (o segundo fator de autenticação estará incompleto).</span><span class="sxs-lookup"><span data-stu-id="f3a0f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="f3a0f-110">O ficheiro de palavra-passe não pode ter mais de 10 MB.</span><span class="sxs-lookup"><span data-stu-id="f3a0f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="f3a0f-111">Utilize uma palavra-passe por linha e inclua uma linha em branco (sinal de retorno) após a última palavra-passe na lista.</span><span class="sxs-lookup"><span data-stu-id="f3a0f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="f3a0f-112">Informações importantes sobre as **simulações de anexação de Phishing spear:**</span><span class="sxs-lookup"><span data-stu-id="f3a0f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="f3a0f-113">Por predeleção, não pode fornecer um valor personalizado para o URL do servidor de início de sessão de **Phishing.**</span><span class="sxs-lookup"><span data-stu-id="f3a0f-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="f3a0f-114">Se um destinatário [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) utilizar o adicionar Ativar a Mensagem do Relatório para denunciar a mensagem como phishing, poderá não receber alertas da mensagem (porque se trata de um ataque simulado).</span><span class="sxs-lookup"><span data-stu-id="f3a0f-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="f3a0f-115">Relatórios: quando o ataque simulado estiver concluído, pode clicar em Detalhes **do Ataque** para ver o relatório.</span><span class="sxs-lookup"><span data-stu-id="f3a0f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="f3a0f-116">Para obter instruções detalhadas e novas funcionalidades no Simulador de Ataque, consulte [Simulador](/microsoft-365/security/office-365-security/attack-simulator)de Ataque Microsoft 365 .</span><span class="sxs-lookup"><span data-stu-id="f3a0f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
