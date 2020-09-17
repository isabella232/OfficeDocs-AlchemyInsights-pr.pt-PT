---
title: como importar-nk2-ficheiros
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780070"
---
# <a name="how-to-import-nk2-files"></a>Como importar ficheiros .nk2 

Quando inicia o Microsoft Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para o Microsoft 365 pela primeira vez, o seu cache de apelido (armazenado no perfil *profilename*.nk2) é importado para uma mensagem escondida na sua loja de mensagens padrão.

Para importar ficheiros .nk2 para o Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para o Microsoft 365, certifique-se de que o ficheiro .nk2 está na seguinte pasta: %appdata%\Microsoft\Outlook

**Nota:** O ficheiro .nk2 deve ter o mesmo nome que o seu perfil atual do Outlook 2013 ou do Outlook 2016. Por predefinição, o nome do perfil é "Outlook". Para verificar o nome do perfil, siga estes passos: 
1. Clique em **Iniciar** e, em seguida, clique em **Painel de Controlo**.
2. Clique duas **vezes no Correio.**
3. Na caixa de diálogo de configuração de correio, selecione **'Mostrar Perfis'.**
4. Selecione **Start**  >  **Run**.
5. Na **caixa Aberta,** escreva *outlook.exe /importnk2,* e, em seguida, selecione **OK**. 

Depois de importar o ficheiro .nk2, o conteúdo do ficheiro é fundido na cache de apelido existente armazenada na sua caixa de correio.

**Nota**: O ficheiro .nk2 é renomeado com uma extensão de nome de ficheiro .old da próxima vez que iniciar o Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para o Microsoft 365. Se quiser re importar o ficheiro .nk2, retire primeiro a extensão do nome do ficheiro .old.

Para obter mais informações, consulte [Importar ou copiar a Lista Auto-Completa para outro computador](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).