---
title: 902 (Erros de sincronização devido a objetos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998805"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erros de sincronização devido a objetos duplicados

Poderá receber uma das seguintes mensagens de erro quando a sincronização de diretórios terminar em Microsoft 365:

- Não é possível atualizar este objeto no Microsoft Online Services porque os seguintes atributos associados a este objeto têm valores que podem já estar associados a outro objeto no seu diretório local.

- Já existe um objeto sincronizado com o mesmo endereço proxy no seu diretório do Microsoft Online Services.

- Não é possível atualizar este objeto porque os seguintes atributos associados a este objeto têm valores que podem já estar associados a outro objeto nos seus serviços de diretório local: UserPrincipalName.

Para identificar e corrigir o problema, transfira e execute a Ferramenta de Remediação de Erros [IdFix dirSync.](https://github.com/Microsoft/idfix)

Para obter mais informações, consulte [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
