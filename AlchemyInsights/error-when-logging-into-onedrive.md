---
title: 0x8004de40 erro ao iniciar o OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946590"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 erro ao iniciar o OneDrive

Se receber uma mensagem de **0x8004de40** ao entrar no OneDrive, re iniciar o computador quando estiver ligado ao domínio da sua escola ou emprego. Se receber este erro após reiniciar, experimente o seguinte quando estiver ligado ao domínio da sua escola ou emprego:

1. Clique em Iniciar e  escreva **cmd** ou comando na caixa de pesquisa, clique com o botão direito do rato na aplicação de comandos e selecione **Executar como administrador.** Se lhe for solicitada uma palavra-passe de administrador ou uma confirmação, escreva a palavra-passe ou clique em **Permitir**.  

2. Na janela Linha de Comandos, escreva **dsregcmd /leave e**  aguarde até o comando ser concluído. Em **seguida, escreva dsregcmd /join** e aguarde até o comando ser concluído.
3. Re reiniciar o computador.
