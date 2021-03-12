---
title: Exemplo Microsoft Defender para a política anti-phishing do Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750793"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="de58b-102">Exemplo Microsoft Defender para a política anti-phishing do Office 365</span><span class="sxs-lookup"><span data-stu-id="de58b-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="de58b-103">Estas definições permitem uma política chamada *Domínio e CEO*.</span><span class="sxs-lookup"><span data-stu-id="de58b-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="de58b-104">Esta política fornece proteção de utilizador e de domínio contra a personificação e, em seguida, aplica a política a todos os e-mails recebidos pelos utilizadores dentro do domínio.</span><span class="sxs-lookup"><span data-stu-id="de58b-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="de58b-105">Em primeiro lugar, adicione as seguintes informações para criar a política:</span><span class="sxs-lookup"><span data-stu-id="de58b-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="de58b-106">**Nome**: **Descrição** do domínio e do CEO : Garante que o CEO e o seu domínio não estão a ser personificados.</span><span class="sxs-lookup"><span data-stu-id="de58b-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="de58b-107">**Aplicado a**: Selecione **O domínio do destinatário é**.</span><span class="sxs-lookup"><span data-stu-id="de58b-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="de58b-108">Em **qualquer um destes**, selecione **Escolha** e, em seguida, selecione um domínio.</span><span class="sxs-lookup"><span data-stu-id="de58b-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="de58b-109">Selecione **+ Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="de58b-109">Select **+ Add**.</span></span> <span data-ttu-id="de58b-110">Selecione a caixa de verificação ao lado do nome do domínio na lista (por exemplo, *contoso.com*), e, em seguida, selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="de58b-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="de58b-111">Selecione **Feito**.</span><span class="sxs-lookup"><span data-stu-id="de58b-111">Select **Done**.</span></span>
- <span data-ttu-id="de58b-112">Após a criação da apólice, pode afinar a política utilizando as seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="de58b-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="de58b-113">**Adicione utilizadores para proteger:** Para este exemplo, adicione o endereço de e-mail do CEO, no mínimo.</span><span class="sxs-lookup"><span data-stu-id="de58b-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="de58b-114">**Adicionar domínios para proteger:** Adicione o domínio organizacional que inclui o escritório do CEO.</span><span class="sxs-lookup"><span data-stu-id="de58b-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="de58b-115">**Escolha as ações**: Para **se o e-mail for enviado por um utilizador personificado,** selecione **Redirecionar a mensagem para outro endereço de e-mail** e, em seguida, insira o endereço de e-mail do administrador de segurança (por exemplo, *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="de58b-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="de58b-116">Para **se o e-mail for enviado por um domínio personificado,** selecione **Quarantine a mensagem**.</span><span class="sxs-lookup"><span data-stu-id="de58b-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="de58b-117">**Inteligência da caixa de** correio : Por padrão, esta opção é selecionada quando cria uma nova política anti-phishing.</span><span class="sxs-lookup"><span data-stu-id="de58b-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="de58b-118">Deixe esta definição **On** para obter os melhores resultados.</span><span class="sxs-lookup"><span data-stu-id="de58b-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="de58b-119">**Adicionar remetentes e domínios fidedignos:** Para este exemplo, não defina nenhuma sobreposição.</span><span class="sxs-lookup"><span data-stu-id="de58b-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="de58b-120">Depois de rever as definições, **selecione Criar esta política** ou **Guardar,** conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="de58b-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="de58b-121">Para saber mais, consulte [as políticas anti-phishing na Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="de58b-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
