---
title: As etiquetas de sensibilidade não são apresentadas
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061443"
---
# <a name="sensitivity-labels-not-appearing"></a>As etiquetas de sensibilidade não são apresentadas

As etiquetas de sensibilidade permitem-lhe classificar e ajudar a proteger os seus conteúdos confidenciais. Podem ser criadas no Centro de Conformidade do Centro de Conformidade do Microsoft 365, no Microsoft 365 ou no Centro de Conformidade do Microsoft 365 & em Etiquetas de > de Segurança do >. Para saber mais sobre esta funcionalidade, consulte [o artigo Visão geral das etiquetas de sensibilidade.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Se tiver configurado as etiquetas de sensibilidade, mas estas não estiverem a ser apresentadas nas aplicações Microsoft 365, verifique o seguinte:

- Confirme que a etiqueta de sensibilidade [foi publicada](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) para os utilizadores e grupos que pretende.

- Confirme que o utilizador está a utilizar uma aplicação que suporta etiquetas de confidencialidade – consulte [etiquetas de confidencialidade no seu documento.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Se estiver a [migrar etiquetas do Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)tenha em atenção as considerações aqui [enumeradas.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Suporte para a prevenção de perda de dados (DLP): Atualmente, apenas as etiquetas de retenção podem ser utilizadas como uma condição nas políticas DLP.  O suporte para etiquetas de sensibilidade numa política DLP ainda não está disponível, mas estamos a trabalhar para o resolver.

- Quando a encriptação estiver ativada numa etiqueta de sensibilidade, pode escolher:
    - Atribuir permissões agora
    - Permitir que os utilizadores atribuim permissões


Para obter mais informações sobre possíveis problemas, [consulte Problemas conhecidos com etiquetas de confidencialidade.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)