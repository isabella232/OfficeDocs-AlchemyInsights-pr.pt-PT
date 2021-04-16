---
title: 0x8004de40 erro ao lançar o OneDrive
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
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813663"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 erro ao lançar o OneDrive

Se receber um erro **0x8004de40** ao iniciar sessão no OneDrive, reinicie o computador enquanto estiver ligado ao seu trabalho ou domínio escolar. Se receber este erro após o reinício, experimente isto enquanto está ligado ao seu trabalho ou domínio escolar:

1. Clique em Iniciar e **digite cmd** ou pedido de **comando**  na caixa de pesquisa, clique com o botão direito na aplicação de pedido de comando e selecione  **Executar como administrador**. Se for solicitado para uma palavra-passe do administrador ou para uma confirmação, digite a palavra-passe ou clique em **Permitir**.  

2. Na janela 'Pedido de Comando', escreva **/saia**  e aguarde que o comando esteja concluído. Em **seguida, escreva dsregcmd /junte-se** e aguarde que o comando esteja completo.
3. Reinicie o seu computador.
