---
title: A writeback da palavra-passe não está a funcionar
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243519"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="1cca9-102">A writeback da palavra-passe não está a funcionar</span><span class="sxs-lookup"><span data-stu-id="1cca9-102">Password Writeback is not working</span></span>

<span data-ttu-id="1cca9-103">**Estou com problemas em configurar a gravação de passwords.**</span><span class="sxs-lookup"><span data-stu-id="1cca9-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="1cca9-104">A gravação de palavra-passe é uma característica premium.</span><span class="sxs-lookup"><span data-stu-id="1cca9-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="1cca9-105">Certifique-se de que compreende os requisitos de licenciamento:</span><span class="sxs-lookup"><span data-stu-id="1cca9-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="1cca9-106">Deve ter pelo menos uma licença atribuída na sua organização</span><span class="sxs-lookup"><span data-stu-id="1cca9-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="1cca9-107">**Utilizadores da Cloud -** Qualquer Office 365 (O365) pagou SKU, ou Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="1cca9-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="1cca9-108">**Utilizadores em nuvem e/ou no local** - Azure AD Premium P1 ou P2, Mobilidade Empresarial + Segurança (EMS) ou Empresa Produtiva Segura (SPE)</span><span class="sxs-lookup"><span data-stu-id="1cca9-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="1cca9-109">Para saber mais sobre os requisitos de licenciamento, consulte [os requisitos de licenciamento para reposição da palavra-passe de autosserviço Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="1cca9-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="1cca9-110">Tem pelo menos uma conta de administrador e uma conta de utilizador de teste com uma das licenças apropriadas.</span><span class="sxs-lookup"><span data-stu-id="1cca9-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="1cca9-111">Tem de ligar o Azure AD Connect ao Emulador do Controlador de Domínio Primário para que a gravação da palavra-passe funcione.</span><span class="sxs-lookup"><span data-stu-id="1cca9-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="1cca9-112">Pode configurar o Azure AD Connect para utilizar um Controlador de Domínio Primário clicando nas **propriedades** do conector de sincronização do Diretório Ativo e, em seguida, selecionando **divisórias de diretório de configuração**.</span><span class="sxs-lookup"><span data-stu-id="1cca9-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="1cca9-113">A partir daí, procure a secção de **definições de conexão do controlador de domínio** e verifique a caixa intitulada **apenas utilizar controladores de domínio preferidos**.</span><span class="sxs-lookup"><span data-stu-id="1cca9-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="1cca9-114">Se o DC preferido não for um emulador PDC, o Azure AD Connect ainda contactará o PDC para obter a gravação de passwords.</span><span class="sxs-lookup"><span data-stu-id="1cca9-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="1cca9-115">O reset da palavra-passe foi configurado e ativado no seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="1cca9-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="1cca9-116">Para obter mais informações, consulte [Ativar os utilizadores para redefinir as suas palavras-passe AD Azure](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="1cca9-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="1cca9-117">Certifique-se de que a conta de administrador utilizada para ativar o Writeback de Password é uma conta de administrador em nuvem (criada em AD Azure e não no local AD)</span><span class="sxs-lookup"><span data-stu-id="1cca9-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="1cca9-118">Tem uma implementação de AD de uma única ou multi-floresta no local com o Windows Server 2008 R2, Windows Server 2012 ou Windows Server 2012 R2 com os mais recentes pacotes de serviços instalados</span><span class="sxs-lookup"><span data-stu-id="1cca9-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="1cca9-119">Tem a ferramenta Azure AD Connect instalada e preparou o seu ambiente AD para sincronização na nuvem.</span><span class="sxs-lookup"><span data-stu-id="1cca9-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="1cca9-120">Antes de testar a gravação da palavra-passe, certifique-se de que primeiro completa uma importação completa e sincronização completa tanto da AD como da AZure AD no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1cca9-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="1cca9-121">Para saber mais, veja como fazer uma [sincronização completa e importação completa em Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="1cca9-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="1cca9-122">**Estou tendo um problema com a conectividade de gravação de palavra-passe**</span><span class="sxs-lookup"><span data-stu-id="1cca9-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="1cca9-123">Faça o download e ative a versão mais recente do [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="1cca9-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="1cca9-124">Configuração de firewall: A ferramenta Azure AD Connect (1.1.443 ou superior) necessitará de acesso **HTTPS de saída** para:</span><span class="sxs-lookup"><span data-stu-id="1cca9-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="1cca9-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1cca9-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="1cca9-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="1cca9-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="1cca9-127">Deixe que as ligações inativas permaneçam durante pelo menos 2-3 minutos</span><span class="sxs-lookup"><span data-stu-id="1cca9-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="1cca9-128">**Ainda estou com problemas com a gravação da palavra-passe.**</span><span class="sxs-lookup"><span data-stu-id="1cca9-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="1cca9-129">Se ainda tiver dificuldades, tente desativar e voltar a ativar o serviço de writeback de palavra-passe na ferramenta Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="1cca9-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="1cca9-130">Para saber mais, veja como [desativar e ativar o writeback de palavras-passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="1cca9-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
