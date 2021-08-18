---
title: Resolver problemas de instalação MDATP num Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091064"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Resolver problemas de instalação MDATP num Mac

Se a instalação manual falhar, a **página** Resumo do assistente de instalação apresenta o seguinte erro:

"Ocorreu um erro durante a instalação. O Instalador encontrou um erro que fez com que a instalação falhasse. Contacte o fabricante do software para obter assistência."

Para implementar MDM, a página também apresenta uma falha de instalação genérica.

Apesar de não apresentarmos erros exatos aos utilizadores finais, mantemos um ficheiro de registo com o progresso da instalação, em **/Library/Logs/Microsoft/mdatp/install.log.** Cada sessão de instalação é acrescentada a este ficheiro de registo. Para saída apenas da última sessão de instalação, utilize `sed` .

Para saber mais, consulte [Remoção de problemas de instalação do Microsoft Defender ATP para Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
