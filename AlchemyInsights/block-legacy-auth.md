---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820189"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="9a50e-102">Bloquear a autenticação do legado</span><span class="sxs-lookup"><span data-stu-id="9a50e-102">Blocking legacy authentication</span></span>

<span data-ttu-id="9a50e-103">Autenticação de legado é um termo que se refere a um pedido de autenticação feito por:</span><span class="sxs-lookup"><span data-stu-id="9a50e-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="9a50e-104">Clientes antigos do Office que não utilizam a autenticação moderna (por exemplo, cliente do Office 2010).</span><span class="sxs-lookup"><span data-stu-id="9a50e-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="9a50e-105">Qualquer cliente que utilize protocolos de correio antigos como IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="9a50e-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="9a50e-106">Para obter mais informações sobre o bloqueio da autenticação do legado e a autenticação moderna, consulte a [autenticação do legado Blocking](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="9a50e-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="9a50e-107">As falhas de segurança no Azure Ative Directory (Azure AD) facilitam a segurança e ajudam a proteger a sua organização.</span><span class="sxs-lookup"><span data-stu-id="9a50e-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="9a50e-108">As falhas de segurança contêm definições de segurança pré-configuradas para ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="9a50e-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="9a50e-109">Para obter mais informações sobre falhas de segurança, consulte [o que são falhas de segurança?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="9a50e-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="9a50e-110">**Nota:** Se o seu inquilino foi criado no dia 22 de outubro de 2019, é possível que esteja a experimentar o novo comportamento de segurança por defeito e já tenha incumprimentos de segurança ativados no seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="9a50e-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="9a50e-111">Num esforço para proteger todos os nossos utilizadores, estão a ser lançados incumprimentos de segurança a todos os novos inquilinos criados.</span><span class="sxs-lookup"><span data-stu-id="9a50e-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
