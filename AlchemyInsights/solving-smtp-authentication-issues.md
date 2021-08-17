---
title: Ativar a autenticação e reação de problemas SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890445"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Ativar a autenticação e reação de problemas SMTP

Se quiser ativar a autenticação SMTP para uma caixa de correio ou se estiver a obter um "Cliente não autenticado", Erro "Autenticação sem sucesso" ou "SmtpClientAuthentication" com o código 5.7.57 ou 5.7.3 ou 5.7.139 quando tenta reenviar o e-mail ao autenticar um dispositivo ou aplicação com o Microsoft 365, efetue estas três ações para resolver o problema:

1. Desativar as [predefinições de](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) segurança do Azure ao ativar as **predefinições de segurança** para **Não.**

    a. Inscreva-se no portal do Azure como administrador de segurança, administrador de Acesso Condicional ou administrador global.<BR/>
    b. Navegue até Azure Active Directory > **Propriedades.**<BR/>
    c. **Selecione Gerir predefinições de segurança**.<BR/>
    d. Defina **Ativar as predefinições** de **segurança para Não**.<BR/>
    e. Seleccione **Guardar**.

2. [Ative a submissão SMTP de](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) Cliente na caixa de correio licenciada.

    a. A partir do centro de administração do Microsoft 365, vá para **Utilizadores Ativos** e selecione o utilizador.<BR/>
    b. Vá para o separador Correio e, em Aplicações **de e-mail**, selecione **Gerir aplicações de e-mail**.<BR/>
    d. Certifique-se **de que O SMTP Autenticado** está se des marcada (ativado).<BR/>
    e. **Selecione Guardar alterações**.<BR/>

3. [Desativar a Autenticação Multifatores (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) na caixa de correio licenciada.

    a. Vá para o centro de administração do Microsoft 365 e, no menu de navegação esquerdo, selecione **Utilizadores**  >  **Ativos.**<BR/>
    b. **Selecione Autenticação multifator.**<BR/>
    c. Selecione o utilizador e **desativar a austeridade Multifator.**<BR/>
