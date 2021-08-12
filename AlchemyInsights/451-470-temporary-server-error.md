---
title: 451 4.7.0 Erro temporário do servidor. Tente novamente mais tarde. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812587"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Erro temporário do servidor. Tente novamente mais tarde. PRX4

Poderá detetar um problema ao enviar um e-mail através do Smarthost "smtp.office365.com" através do método de Submissão de Cliente SMTP e receber a mensagem de erro: "451 4.7.0 Erro temporário do servidor. Tente novamente mais tarde. O PRX4 é principalmente temporário." 

Certifique-se de que não está a utilizar uma caixa de correio partilhada para a Submissão de Cliente SMTP, uma vez que o método de Submissão de cliente SMTP necessita de uma caixa de correio licenciada para enviar correio. No entanto, se não estiver a utilizar uma caixa de correio partilhada e o problema persistir, verifique o seguinte:

1. Ative a submissão SMTP de Cliente na caixa de correio licenciada que está a ser utilizada ao executar este comando do PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OU

    1. Vá para o centro de administração do Microsoft 365 > **utilizadores ativos** e selecione o utilizador.
    1. Vá para o separador Correio > **aplicações de e->** selecione **Gerir aplicações de e-mail**. 
    1. Certifique-se de **que a definição SMTP Autenticado** está marcada (ativada).
    1. **Selecione Guardar alterações**.
    
    Para ativar a Autenticação SMTP para uma organização inteira, execute este comando:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Nota:** Por motivos de segurança, recomenda-se que ative a Autenticação SMTP apenas para a caixa de correio a ser utilizada. A definição de nível de utilizador substitui a definição ao nível da organização.

2. Desativar as Predefinições de Segurança do Azure ao ativar **as predefinições de segurança** para **Não:**

    1. Inscreva-se no portal do Azure como administrador de segurança, administrador de Acesso Condicional ou administrador global.
    1. Navegue até às Azure Active Directory >**  e selecione** Gerir **predefinições de segurança.**
    1. Defina o **alternar Ativar predefinições** de segurança para **Não.**
    1. Seleccione **Guardar**.

3. Desativar a Autenticação Multifatores (MFA) na caixa de correio licenciada a ser utilizada.

    1. Vá para o centro de administração do Microsoft 365 e, no menu de navegação esquerdo, selecionar **Utilizadores**  >  **Ativos.**
    1. Na página Utilizadores **ativos,** selecionar **Autenticação multifatores.**
    1. Selecione o utilizador e desativar **a autenticação multifator.**

