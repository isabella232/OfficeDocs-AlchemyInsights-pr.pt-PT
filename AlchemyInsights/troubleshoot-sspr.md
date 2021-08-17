---
title: Remoção de Problemas de SSPR
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038969"
---
# <a name="troubleshoot-sspr"></a>Remoção de Problemas de SSPR

**Estou a ter problemas com a configuração da reposição da palavra-passe**

- Se for administrador e estiver à procura de como ativar a reposição de palavra-passe self-service, consulte [Tutorial ativar o SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)para configurar a reposição de palavras-passe para a sua organização. Poderá também querer rever os [requisitos de licenciamento.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Tem de ter, pelo menos, uma licença atribuída na sua organização.
    - **Apenas utilizadores na nuvem** – Office 365 SKU pago (O365) ou Azure AD Basic
    - **Utilizadores da nuvem e/ou** no local : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
- Para obter perguntas adicionais sobre a reposição de palavras-passe auto-serviço, reveja [as nossas FAQ.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Estou a receber uma mensagem de erro**

Reveja este artigo para encontrar erros comuns e as respetivas soluções: Reposição de [palavra-passe self-service](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Estou a ter um problema com a minha política de reposição de palavras-passe**

- Se a sua política de reposição de palavras-passe não estiver a comportar-se conforme esperado ou se tiver perguntas sobre políticas de reposição de palavras-passe, reveja este artigo: Políticas e restrições de palavras-passe [em Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- As políticas de reposição de palavras-passe não se aplicam a administradores. A Microsoft impõe uma forte política de reposição de palavra-passe predefinida de dois gates para qualquer função de administrador do Azure. Certifique-se de que está a testar com um utilizador que não é administrador. Para obter mais informações sobre a política de reposição de administrador, consulte este artigo: [Diferenças de políticas de reposição de administrador.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Não quero que os meus utilizadores registe informações de segurança adicionais para repor a palavra-passe**

Pode pré-preencher dados (atributos de e-mail e telefone) para os seus utilizadores através de uma API, PowerShell ou Azure AD Ligação. Para saber como ler:

- [Implementar a reposição de palavra-passe sem que os utilizadores se registe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Que dados são utilizados pela reposição de palavra-passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Quero que os meus utilizadores registem as informações de segurança adicionais para repor a palavra-passe**

1. Registe as informações de segurança dos seus utilizadores para reporem a palavra-passe de utentes direcionados para [o aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Após a preenchimento dos dados para o utilizador (pelo utilizador ou pelo administrador), direcionar o seu utilizador para o [aka.ms/sspr](https://passwordreset.microsoftonline.com/) para que os seus utilizadores possam repor as suas próprias palavras-passe.
1. Se os utilizadores continuarem a ter problemas, provavelmente já estão **federados ou** os utilizadores **sincronizados com hashs** de palavras-passe. Isto significa que é provável que haja um problema com o serviço Writeback de Palavra-passe.