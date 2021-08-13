---
title: Limitações de etiquetas de sensibilidade para Office ficheiros no SharePoint e no OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813163"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Limitações de etiquetas de sensibilidade para Office ficheiros no SharePoint e no OneDrive

Ao ativar etiquetas de sensibilidade Office ficheiros no SharePoint e no OneDrive, tenha em atenção os requisitos e limitações, que incluem:

- O SharePoint e o OneDrive não conseguem processar alguns ficheiros etiquetados e encriptados Office partir de Office plicações de ambiente de trabalho quando os ficheiros contêm dados do PowerQuery, dados armazenados por add-ins personalizados ou peças XML personalizadas.
- O SharePoint OneDrive não aplicam etiquetas de confidencialidade automaticamente aos ficheiros existentes que já encriptou com etiquetas Azure Information Protection (AIP). Para aplicar etiquetas de sensibilidade a ficheiros encriptados: 
    - Certifique-se de que as etiquetas AIP foram migradas e publicadas no Microsoft 365 de Conformidade.
    - Transfira os ficheiros etiquetados e, em seguida, carrege-os para a localização original OneDrive SharePoint.
- Para documentos encriptados, a impressão não é suportada.

Para obter detalhes adicionais sobre limitações, consulte Ativar etiquetas de [Office ficheiros no SharePoint e no OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
