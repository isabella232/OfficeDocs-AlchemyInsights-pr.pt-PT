---
title: Corrigir problemas comuns com a formatação de registos DKIM
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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930072"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Corrigir problemas comuns com a formatação de registos DKIM

A maioria dos problemas de configuração do DKIM estão relacionados com registos DNS incorretos.

Para corrigir os problemas de configuração do DKIM, verifique se o registo DKIM CNAME **(e** não um registo TXT) está formatado corretamente. Para obter mais informações, consulte O que precisa de fazer para configurar [manualmente o DKIM no Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Se precisar de ajuda com os registos DNS em geral, consulte Criar registos DNS em qualquer fornecedor de anfitrião [DNS para Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Após criar ou atualizar os seus registos DKIM DNS no serviço de registo DNS do seu domínio, terá de aguardar que os registos DNS propaguem.
