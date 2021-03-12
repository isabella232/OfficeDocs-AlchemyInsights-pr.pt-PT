---
title: Corrigir problemas comuns com formatação de registo dKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750760"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Corrigir problemas comuns com formatação de registo dKIM

A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos.

Para corrigir os problemas de configuração do DKIM, verifique se o registo DKIM CNAME **(não** um registo TXT) está formatado corretamente. Para mais informações, consulte [o que precisa de fazer para configurar manualmente o DKIM no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Se precisar de ajuda com registos DNS em geral, consulte [crie registos DNS em qualquer fornecedor de hospedagem DNS para o Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Depois de criar ou atualizar os seus registos DKIM DNS no serviço de hospedagem DNS para o seu domínio, terá de esperar que os registos DNS se propaguem.
