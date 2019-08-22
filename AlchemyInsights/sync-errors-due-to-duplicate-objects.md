---
title: 902 (erros de sincronização devido a objectos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507426"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erros de sincronização devido a objectos duplicados

Poderá receber uma das seguintes mensagens de erro quando concluir a sincronização de directórios no Office 365:

- Não é possível actualizar este objecto no Microsoft Online Services porque os seguintes atributos associados a este objecto tem valores que já esteja associados a outro objecto no directório local.

- Já existe um objecto sincronizado com o mesmo endereço de proxy no directório do Microsoft Online Services.

- Não é possível actualizar este objecto porque os seguintes atributos associados a este objecto tem valores que já esteja associados a outro objecto os serviços de directório local: UserPrincipalName.

Para identificar e corrigir o problema, transfira e execute a [Ferramenta de reparação do IdFix DirSync erros](https://www.microsoft.com/download/details.aspx?id=36832).

Para mais informações, consulte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
