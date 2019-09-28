---
title: 2681 simulador de ataque no Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305342"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="ad45e-102">Simulador de ataque no Office 365</span><span class="sxs-lookup"><span data-stu-id="ad45e-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="ad45e-103">Você está faltando simulador de ataque?</span><span class="sxs-lookup"><span data-stu-id="ad45e-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="ad45e-104">O simulador de ataque requer o **office 365 Advanced Threat Protection Plan 2 (plano ATP 2)** ou o **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="ad45e-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="ad45e-105">O simulador de ataque **não** está incluído no Office 365 Advanced Threat Protection Plan 1 (plano ATP 1), Office 365 Enterprise E3 ou qualquer assinatura do Office 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ad45e-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="ad45e-106">A conta que você usa para iniciar ataques simulados requer permissões de administrador global ou de segurança e autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="ad45e-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="ad45e-107">Para obter mais informações sobre os requisitos do simulador de ataque, consulte [Este tópico](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="ad45e-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="ad45e-108">Coisas importantes para saber sobre **Brute Force** simulações de ataque de senha:</span><span class="sxs-lookup"><span data-stu-id="ad45e-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="ad45e-109">Se a conta de destino tiver a MFA ativada e a senha foi adivinhada corretamente, a conta não será mostra como comprometida (o segundo fator de autenticação será incompleto).</span><span class="sxs-lookup"><span data-stu-id="ad45e-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="ad45e-110">O arquivo de senha não pode ser maior que 10 MB.</span><span class="sxs-lookup"><span data-stu-id="ad45e-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="ad45e-111">Use uma senha por linha e inclua uma linha em branco (retorno de carro) após a última senha na lista.</span><span class="sxs-lookup"><span data-stu-id="ad45e-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="ad45e-112">Coisas importantes a saber sobre simulações de **lança de phishing** :</span><span class="sxs-lookup"><span data-stu-id="ad45e-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="ad45e-113">Por predefinição, não pode fornecer um valor personalizado para a **URL do servidor de início de sessão de phishing**.</span><span class="sxs-lookup"><span data-stu-id="ad45e-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="ad45e-114">Se um destinatário usar a [opção Habilitar o suplemento relatar mensagem](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) para relatar a mensagem como phishing, talvez você não receba alertas para a mensagem (porque este é um ataque simulado).</span><span class="sxs-lookup"><span data-stu-id="ad45e-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="ad45e-115">Relatórios: após a conclusão do ataque simulado, você pode clicar em **detalhes de ataque** para ver o relatório.</span><span class="sxs-lookup"><span data-stu-id="ad45e-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="ad45e-116">Para obter instruções detalhadas e novos recursos no simulador de ataque, consulte [simulador de ataque no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="ad45e-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
