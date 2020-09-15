---
title: 'Erro: As regras deste computador não coincidem'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690974"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erro: As regras deste computador não coincidem

Para ver o estado atualizado deste problema conhecido, consulte [as regras deste computador que não correspondem às regras da Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

A Equipa Outlook implementou uma correção na Build 12928.10000. A correção já está no Insider Fast e irá para o Monthly Channel no final de junho de 2020. Uma vez que tenha a construção fixa, poderá obter o pedido "Quais as regras que quer manter" uma última vez. Escolha o Servidor quando solicitado e volte ao Outlook e volte a ativar quaisquer regras que foram desativadas.

Até que a correção esteja disponível, utilize a seguinte solução:

**Solução alternativa**: Em relatórios recentes, o problema ocorreu para aqueles que apenas criaram regras de clientes no ambiente de trabalho do Outlook. Se continuar a deparar-se com o problema, considere eliminar as regras e, em seguida, criar e editar regras apenas na OWA (Outlook Web App) até que o problema seja resolvido.

Se não conseguir eliminar as regras manualmente, pode executar um comando Outlook quando iniciar o Outlook executando Outlook.exe /regras de limpeza. Isto eliminará as regras do cliente e do servidor. Eliminará todas as regras para todas as contas do Perfil outlook. Este comando está ainda documentado no artigo de comutações da linha de comando.

