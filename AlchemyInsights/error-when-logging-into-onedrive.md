---
title: Erro 0x8004de40 ao lançar o OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823114"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>Erro 0x8004de40 ao lançar o OneDrive

Se receber um erro **0x8004de40** ao iniciar sessão no OneDrive, reinicie o computador enquanto estiver ligado ao seu trabalho ou domínio escolar. Se receber este erro após o reinício, experimente isto enquanto está ligado ao seu trabalho ou domínio escolar:

1. Clique em Iniciar e **digite cmd** ou pedido de **comando**  na caixa de pesquisa, clique com o botão direito na aplicação de pedido de comando e selecione  **Executar como administrador** . Se for solicitado para uma palavra-passe do administrador ou para uma confirmação, digite a palavra-passe ou clique em **Permitir** .  

2. Na janela 'Pedido de Comando', escreva **/saia**  e aguarde que o comando esteja concluído. Em **seguida, escreva dsregcmd /junte-se** e aguarde que o comando esteja completo.
3. Reinicie o seu computador.
