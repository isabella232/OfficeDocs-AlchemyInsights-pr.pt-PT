---
title: Simulador de ataque 2681 na Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713477"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="2598d-102">Simulador de ataque na Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2598d-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="2598d-103">Estás a perder o Simulador de Ataque?</span><span class="sxs-lookup"><span data-stu-id="2598d-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="2598d-104">O Simulador de Ataque requer o **Office 365 Advanced Threat Protection Plan 2 (PLANO ATP 2)** ou **o Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="2598d-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="2598d-105">O Attack Simulator **não** está incluído no Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 ou em quaisquer Aplicações Microsoft 365 para subscrições de negócios.</span><span class="sxs-lookup"><span data-stu-id="2598d-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="2598d-106">A conta que utiliza para lançar ataques simulados requer permissões de administrador global ou administrador de segurança e autenticação de vários fatores (MFA).</span><span class="sxs-lookup"><span data-stu-id="2598d-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="2598d-107">Para mais informações sobre os requisitos do Simulador de Ataque, consulte [este tópico](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="2598d-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="2598d-108">Coisas importantes a saber sobre simulações de ataque de **palavra-passe** da Força Bruta:</span><span class="sxs-lookup"><span data-stu-id="2598d-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="2598d-109">Se a conta-alvo tiver MFA ativada e a palavra-passe tiver sido adivinho corretamente, a conta não aparecerá como comprometida (o segundo fator de autenticação estará incompleto).</span><span class="sxs-lookup"><span data-stu-id="2598d-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="2598d-110">O ficheiro de senha não pode ser maior que 10 MB.</span><span class="sxs-lookup"><span data-stu-id="2598d-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="2598d-111">Utilize uma palavra-passe por linha e inclua uma linha em branco (retorno do transporte) após a última palavra-passe da lista.</span><span class="sxs-lookup"><span data-stu-id="2598d-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="2598d-112">Coisas importantes a saber sobre **spear phishing** anexam simulações:</span><span class="sxs-lookup"><span data-stu-id="2598d-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="2598d-113">Por design, não é possível fornecer um valor personalizado para o URL do servidor de **login**de phishing .</span><span class="sxs-lookup"><span data-stu-id="2598d-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="2598d-114">Se um destinatário utilizar o [add-in Enable the Report Message](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) para relatar a mensagem como phishing, poderá não receber alertas para a mensagem (porque se trata de um ataque simulado).</span><span class="sxs-lookup"><span data-stu-id="2598d-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="2598d-115">Relatórios: Após o ataque simulado estar completo, pode clicar em Detalhes de **Ataque** para ver o relatório.</span><span class="sxs-lookup"><span data-stu-id="2598d-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="2598d-116">Para obter instruções detalhadas e novas funcionalidades no Simulador de Ataque, consulte [o Simulador de Ataque na Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="2598d-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
