---
title: Iniciar sessão no Windows 10 sem usar uma senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588291"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Iniciar sessão no Windows 10 sem usar uma senha

Para evitar ter de escrever uma palavra-passe no arranque do Windows, recomendamos que utilize uma das opções de entrada segura do Windows Hello, como um PIN, reconhecimento facial ou impressão digital, se disponível. Se realmente quiser desativar o acesso seguro, consulte as instruções "Iniciar automaticamente o sessão no Windows 10" abaixo.

**Alternativas Secure Windows Hello à palavra-passe da conta**

Vá a **Definições > Contas > opções de iniciar sessão** (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)). As opções de inscrição disponíveis serão listadas. Por exemplo:

![Opções de inscrição.](media/sign-in-options.png)

Clique ou toque numa das opções para configurá-lo. Da próxima vez que iniciar ou desbloquear o Windows, poderá utilizar a nova opção em vez de uma palavra-passe. 

**Iniciar sessão automática no Windows 10**

**Nota:** O início automático é conveniente, mas introduz um risco de segurança, especialmente se o seu PC estiver acessível por várias pessoas. 

1. Clique ou toque no botão **Iniciar** na barra de tarefas.

2. Digite **netplwiz** e acerte na tecla Enter para abrir a janela contas do utilizador.

3. Nas **Contas do Utilizador,** clique na conta para a sua assinatura automaticamente quando o Windows começar.

4. Desmarque a caixa de verificação "Os utilizadores devem introduzir um nome de utilizador e uma senha para utilizar este computador".

    ![Os utilizadores devem introduzir uma opção de username e password.](media/users-must-enter-username.png)

5. Clique em **OK**. Será-lhe pedido que introduza e confirme a palavra-passe para a conta selecionada. Clique **em OK** para terminar. Da próxima vez que o Windows 10 começar, iniciará automaticamente o seu início na conta selecionada.
