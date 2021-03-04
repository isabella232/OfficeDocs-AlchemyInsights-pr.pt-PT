---
title: SSPR resolução de problemas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430218"
---
# <a name="troubleshoot-sspr"></a>SSPR resolução de problemas

**Estou a ter problemas em configurar a palavra-passe.**

- Se você é administrador e está à procura de como ativar o reset da palavra-passe de autosserviço, consulte [Tutorial ativar o SSPR,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)para configurar a palavra-passe reiniciada para a sua organização. Também pode querer rever os [requisitos de licenciamento.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Deve ter pelo menos uma licença atribuída na sua organização.
    - **Utilizadores da Cloud -** Qualquer Office 365 (O365) pagou SKU, ou Azure AD Basic
    - **Utilizadores em nuvem e/ou no local** - Azure AD Premium P1 ou P2, Mobilidade Empresarial + Segurança (EMS) ou Empresa Produtiva Segura (SPE)
- Para mais perguntas sobre o reset da palavra-passe de autosserviço, [reveja as nossas FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Estou a receber uma mensagem de erro.**

Reveja este artigo para encontrar erros comuns e suas soluções: [Resolução de autosserviço de resolução de problemas redefinindo a palavra-passe de autosserviço](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Estou tendo um problema com a minha política de reset de senha**

- Se a sua política de reset de palavra-passe não se comportar como esperado, ou se tiver dúvidas sobre políticas de reset de passwords, reveja este artigo: [Políticas de palavra-passe e restrições no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- As políticas de reset de palavra-passe não se aplicam aos administradores. A Microsoft aplica uma forte política de reset de senha de dois prazos para qualquer função de administrador do Azure. Certifique-se de que está a testar com um utilizador que não é administrador. Para obter mais informações sobre a política de reposição do administrador, consulte este artigo: [Administrador repor as diferenças de política](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Não quero que os meus utilizadores registem informações adicionais de segurança para reset de password**

Pode pré-povoar dados (email e atributos de telefone) para os seus utilizadores usando um API, PowerShell ou Azure AD Connect. Para aprender a ler:

- [Implementar a palavra-passe reiniciada sem exigir que os utilizadores se registem](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Que dados são usados por reset de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Quero que os meus utilizadores registem as suas informações de segurança adicionais para reset de password**

1. Que os seus utilizadores registem as suas informações de segurança para a redefinição da palavra-passe de autosserviço, direcionando-os para [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Depois de os dados serem preenchidos para o utilizador (pelo utilizador ou pelo administrador), direcione o utilizador para [aka.ms/sspr](https://passwordreset.microsoftonline.com/) para que os seus utilizadores possam ser capacitados para redefinir as suas próprias palavras-passe.
1. Se os utilizadores ainda estiverem com problemas, é provável que sejam **utilizadores sincronizados** ou sincronizados com **palavras-passe.** Isto significa que há provavelmente um problema com o serviço de writeback de palavra-passe.