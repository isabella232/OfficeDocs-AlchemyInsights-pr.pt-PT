---
title: Inscrever-se no Windows 10 sem utilizar uma palavra-passe
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
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107530"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Inscrever-se no Windows 10 sem utilizar uma palavra-passe

Para evitar ter de escrever uma palavra-passe no arranque do Windows, recomendamos que utilize uma das opções de início de trabalho seguras do Windows Hello, como um PIN, reconhecimento facial ou impressão digital, se disponível. Se quiser mesmo desativar o sinal de segurança, consulte as instruções "In deslocar-se automaticamente para Windows 10".

**Proteger as Windows Hello alternativas à palavra-passe da conta**

Vá para **Definições > Contas > opções de Inscrever-se** (ou clique [aqui).](ms-settings:signinoptions?activationSource=GetHelp) Serão listadas as opções de inscrever-se disponíveis. Por exemplo:

![Opções de inscrever-se.](media/sign-in-options.png)

Clique ou toque numa das opções para configurá-la. Da próxima vez que iniciar ou desbloquear uma Windows, poderá utilizar a nova opção em vez de uma palavra-passe. 

**Inscreva-se automaticamente no Windows 10**

**Nota:** o acesso automático é conveniente, mas apresenta um risco de segurança, especialmente se o PC for acessível por múltiplas pessoas. 

1. Clique ou toque no **botão Iniciar** na Barra de Tarefas.

2. Escreva **netplwiz e** aperte a tecla Enter para abrir a janela Contas de Utilizador.

3. Em **Contas de Utilizador**, clique na conta em que pretende iniciar automaticamente a Windows iniciada.

4. Desloque a caixa de verificação "Os utilizadores têm de introduzir um nome de utilizador e palavra-passe para utilizar este computador".

    ![Os utilizadores têm de introduzir uma opção de nome de utilizador e palavra-passe.](media/users-must-enter-username.png)

5. Clique em **OK**. Ser-lhe-à pedido para introduzir e confirmar a palavra-passe da conta que selecionou. Clique **em OK** para concluir. Da próxima vez Windows 10 inicia, iniciará automaticamente na conta que selecionou.
