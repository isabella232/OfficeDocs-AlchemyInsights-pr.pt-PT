---
title: Não pode aceder a pastas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891760"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>O Outlook não pode ligar-se a pastas públicas

Se o acesso a pasta pública não estiver a funcionar para alguns utilizadores, tente o seguinte:

Ligue-se ao EXO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta de utilizador problemática para combinar o parâmetro numa conta de utilizador em funcionamento.

Exemplo:

Caixa de correio de caixa de correio funcionador [ User] ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Problemas de caixa de correio de \<conjuntoUser -DefaultPublicFolderMailbox valor de comando anterior>

Espere pelo menos uma hora para que a mudança faça efeito.

Se o problema se mantiver, siga [este procedimento](https://aka.ms/pfcte) para resolver problemas de acesso a pastas públicas utilizando o Outlook.