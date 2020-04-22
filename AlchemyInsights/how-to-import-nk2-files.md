---
title: como importar-nk2-ficheiros
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759343"
---
# <a name="how-to-import-nk2-files"></a>Como importar ficheiros .nk2 

Quando iniciar o Microsoft Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para o Microsoft 365 pela primeira vez, o seu cache de apelido (armazenado no *ficheiro profilename*.nk2) é importado para uma mensagem escondida na sua loja de mensagens padrão.

Para importar ficheiros .nk2 para o Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para o Microsoft 365, certifique-se de que o ficheiro .nk2 está na seguinte pasta: %appdata%\Microsoft\Outlook

**Nota:** O ficheiro .nk2 deve ter o mesmo nome do seu perfil atual do Outlook 2013 ou do Outlook 2016. Por padrão, o nome do perfil é "Outlook". Para verificar o nome do perfil, siga estes passos: 
1. Clique em **Iniciar**, e depois clique no **Painel de Controlo**.
2. Correio de **dois**cliques.
3. Na caixa de diálogo mail setup, selecione **Perfis de série**.
4. Selecione **Iniciar** > **execução**.
5. Na caixa **Aberta,** digite *outlook.exe /importnk2*, e, em seguida, selecione **OK**. 

Depois de importar o ficheiro .nk2, o conteúdo do ficheiro é fundido na cache de apelido existente armazenada na sua caixa de correio.

**Nota:** O ficheiro .nk2 é renomeado com uma extensão de nome de ficheiro .old da próxima vez que iniciar o Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para o Microsoft 365. Se quiser reimportar o ficheiro .nk2, remova primeiro a extensão de nome de ficheiro .old.

Para mais informações, consulte [importar ou copiar a Lista Auto-Completa para outro computador](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).