---
title: Não é possível ativar o Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798691"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="8c380-102">Não é possível ativar o Office</span><span class="sxs-lookup"><span data-stu-id="8c380-102">Unable to activate Office</span></span>

<span data-ttu-id="8c380-103">**Nota:** se estiver a utilizar uma versão mais antiga do Windows (por exemplo, o Windows 7), certifique-se de que o TLS 1.2 está ativado como predefinição.</span><span class="sxs-lookup"><span data-stu-id="8c380-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="8c380-104">Para obter mais informações, consulte Update [to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="8c380-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="8c380-105">Verifique se o seu estado de subscrição expirou.</span><span class="sxs-lookup"><span data-stu-id="8c380-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="8c380-106">Certifique-se de que tem uma subscrição que permite licenças de clientes, como o Microsoft 365 Apps para Pequenas e Médias Empresas ou o Microsoft 365 Empresas Premium e [assegure-se de que o utilizador tem uma licença atribuída](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="8c380-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="8c380-107">Certifique-se de que o utilizador está a iniciar sessão no Office com a mesma conta à qual tem a licença atribuída.</span><span class="sxs-lookup"><span data-stu-id="8c380-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="8c380-108">Consulte a [página do Estado de Funcionamento dos Serviços do Office 365](/office365/enterprise/view-service-health) para ver se existem problemas conhecidos com o serviço.</span><span class="sxs-lookup"><span data-stu-id="8c380-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="8c380-109">Verifique as definições da firewall, software antivírus e proxy para confirmar que não estão a bloquear o acesso do Microsoft 365 Apps à internet.</span><span class="sxs-lookup"><span data-stu-id="8c380-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="8c380-110">Consulte [URLs e intervalos de endereços IP do Office 365](/office365/enterprise/urls-and-ip-address-ranges "Intervalos de endereços IP e URLs do Office 365").</span><span class="sxs-lookup"><span data-stu-id="8c380-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="8c380-111">**Sugestão** Em computadores Windows, podemos diagnosticar e corrigir automaticamente vários problemas comuns de início de sessão do Office.</span><span class="sxs-lookup"><span data-stu-id="8c380-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="8c380-112">Transfira e execute o **[Assistente de Recuperação e Suporte da Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para utilizar a nossa ferramenta automatizada.</span><span class="sxs-lookup"><span data-stu-id="8c380-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="8c380-113">Utilize as seguintes ações de resolução de problemas:</span><span class="sxs-lookup"><span data-stu-id="8c380-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="8c380-114">Abra uma aplicação do Office e [termine sessão](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) em quaisquer uma das contas de utilizador existentes.</span><span class="sxs-lookup"><span data-stu-id="8c380-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="8c380-115">[Remova](/microsoft-365/admin/manage/remove-licenses-from-users) e [reatribua](/microsoft-365/admin/manage/assign-licenses-to-users) a licença do Office e, em seguida, [inicie sessão no Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) com a conta de utilizador afetada.</span><span class="sxs-lookup"><span data-stu-id="8c380-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="8c380-116">Execute a [Resolução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="8c380-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="8c380-117">Redefina o estado de ativação do Office</span><span class="sxs-lookup"><span data-stu-id="8c380-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Redefinir o estado de ativação do Office")
- [<span data-ttu-id="8c380-118">Execute uma Reparação Online do Office</span><span class="sxs-lookup"><span data-stu-id="8c380-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="8c380-119">Para soluções adicionais de resolução de problemas, consulte:</span><span class="sxs-lookup"><span data-stu-id="8c380-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="8c380-120">Erros de Produto Não Licenciado e de ativação no Office</span><span class="sxs-lookup"><span data-stu-id="8c380-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="8c380-121">Erro "Desculpe, mas não conseguimos ligar-nos à sua conta. Tente novamente mais tarde" ao ativar o Office</span><span class="sxs-lookup"><span data-stu-id="8c380-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)