---
title: 902 (Erros de sincronização devido a objetos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767146"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erros de sincronização devido a objetos duplicados

Pode receber uma das seguintes mensagens de erro quando a sincronização do diretório terminar no Microsoft 365:

- Incapaz de atualizar este objeto nos Serviços Online da Microsoft porque os seguintes atributos associados a este objeto têm valores que podem já estar associados a outro objeto no seu diretório local.

- Um objeto sincronizado com o mesmo endereço proxy já existe no seu diretório de Serviços Online da Microsoft.

- Incapaz de atualizar este objeto porque os seguintes atributos associados a este objeto têm valores que podem já estar associados a outro objeto nos seus serviços de diretório local: UserPrincipalName.

Para identificar e corrigir o problema, descarregue e execute a [ferramenta de reparação de erros IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Para mais informações, consulte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
