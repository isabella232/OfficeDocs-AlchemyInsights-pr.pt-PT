---
title: how-to-import-nk2-files
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
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043217"
---
# <a name="how-to-import-nk2-files"></a>Como importar ficheiros .nk2 

Quando inicia o Microsoft Outlook 2013, o Outlook 2016, o Outlook 2019 ou o Outlook para Microsoft 365 pela primeira vez, a cache de alcunhas (armazenada no ficheiro .nk2 do nome de perfil) é importada para uma mensagem oculta no seu arquivo de mensagens predefinido.

Para importar ficheiros .nk2 para o Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para Microsoft 365, certifique-se de que o ficheiro .nk2 está na seguinte pasta: %appdata%\Microsoft\Outlook

**Nota:** o ficheiro .nk2 tem de ter o mesmo nome que o seu perfil Outlook 2013 ou Outlook 2016 perfil. Por predefinição, o nome de perfil é "Outlook". Para verificar o nome do perfil, siga estes passos: 
1. Clique em **Iniciar** e, em seguida, clique em **Painel de Controlo**.
2. Faça duplo clique em **Correio.**
3. Na caixa de diálogo Configuração de Correio, selecione **Mostrar Perfis**.
4. Selecione **Iniciar** > **Executar**.
5. Na caixa **Abrir,** escrevaoutlook.exe */importnk2* e, em seguida, selecione **OK.** 

Após importar o ficheiro .nk2, os conteúdos do ficheiro são intercalados com a cache de alcunhas existente armazenada na sua caixa de correio.

**Nota:** o nome do ficheiro .nk2 é renomeado com uma extensão de nome de ficheiro .old da próxima vez que iniciar o Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para Microsoft 365. Se quiser importar o ficheiro .nk2, remova primeiro a extensão de nome de ficheiro .old.

Para obter mais informações, consulte [Importar ou copiar a Lista de Preenção Automática para outro computador.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)