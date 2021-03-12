---
title: Problemas de instalação do MDATP na resolução de problemas num Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749772"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Problemas de instalação do MDATP na resolução de problemas num Mac

Se a instalação manual falhar, a página **resumo** do assistente de instalação mostra o seguinte erro:

"Ocorreu um erro durante a instalação. O Instalador encontrou um erro que fez com que a instalação falhasse. Contacte o fabricante de software para obter assistência."

Para as implementações de MDM, a página também mostra uma falha genérica de instalação.

Embora não apresentemos erros exatos para os utilizadores finais, mantemos um ficheiro de registo com o progresso da instalação, em **/Library/Logs/Microsoft/mdatp/install.log**. Cada sessão de instalação anexa a este ficheiro de registo. Para obter apenas a última sessão de instalação, utilize `sed` .

Para saber mais, consulte [problemas de instalação de resolução de problemas para o Microsoft Defender ATP para Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
