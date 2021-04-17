---
title: Iniciar s-in no Windows 10 sem utilizar uma senha
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830557"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Iniciar s-in no Windows 10 sem utilizar uma senha

Para evitar ter de escrever uma palavra-passe no arranque do Windows, recomendamos que utilize uma das opções de entrada segura do Windows Hello, como um PIN, reconhecimento facial ou impressão digital, se disponível. Se realmente pretender desativar o s-in seguro, consulte as instruções "Iniciar automaticamente o Windows 10" abaixo.

**Secure Windows Hello alternativas à senha de conta**

Aceda a **Definições > Contas > opções de inscrição** (ou clique [aqui).](ms-settings:signinoptions?activationSource=GetHelp) As opções de inscrição disponíveis serão listadas. Por exemplo:

![Opções de inscrição.](media/sign-in-options.png)

Clique ou toque numa das opções para configurá-lo. Da próxima vez que iniciar ou desbloquear o Windows, poderá utilizar a nova opção em vez de uma palavra-passe. 

**Iniciar automaticamente o ó20.**

**Nota:** O acesso automático é conveniente, mas introduz um risco de segurança, especialmente se o seu PC estiver acessível por várias pessoas. 

1. Clique ou toque no botão **Iniciar** na barra de tarefas.

2. Digite **netplwiz** e bata na tecla 'Introduzir' para abrir a janela Contas de Utilizador.

3. Nas **Contas de Utilizador,** clique na conta a que pretende iniciar automaticamente o seu início.

4. Desmarque a caixa de verificação "Os utilizadores devem introduzir um nome de utilizador e uma palavra-passe para utilizar este computador".

    ![Os utilizadores devem introduzir uma opção de nome de utilizador e palavra-passe.](media/users-must-enter-username.png)

5. Clique em **OK**. Ser-lhe-á pedido que introduza e confirme a palavra-passe para a conta que selecionou. Clique **em OK** para terminar. Da próxima vez que o Windows 10 começar, iniciará automaticamente o s registação na conta selecionada.
