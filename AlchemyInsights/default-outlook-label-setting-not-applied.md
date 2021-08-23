---
title: Predefinição Outlook etiqueta não aplicada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455090"
---
# <a name="default-outlook-label-setting-not-applied"></a>Predefinição Outlook etiqueta não aplicada

Se as suas predefinições de etiqueta do Outlook não estiverem a ser aplicadas corretamente e for aplicada uma etiqueta diferente ou não, poderá estar a ter um problema conhecido (MC277818) e deve seguir uma destas 2 opções para resolver o problema:

**Opção 1:**

1. Vá para o Microsoft 365 conformidade do >  >  **Soluções Information Protection.**
1. **Selecione Políticas** de etiquetas e selecione a política de etiquetas que precisa de editar (a definição **OutlookDefaultlabel** não é definida corretamente na política de etiqueta em questão. Execute **Get-labelpolicy** para ver esta definição) e, em seguida, selecione **Editar política**.
1. **Selecione** Seguinte até ver a definição Aplicar esta etiqueta predefinida a e-mails, que está disponível se selecionar Exigir que os utilizadores apliquem uma etiqueta aos e-mails e documentos **dos herdeiros** na caixa de diálogo Definições de política.  
1. Na caixa **de diálogo Aplicar uma etiqueta predefinida** aos documentos, selecionar **Nenhuma** na lista de listas.
1. **Selecione Seguinte** e **Submeter** para guardar as definições da etiqueta.

**Opção 2:**

No [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)do Centro de Conformidade e Segurança, utilize o comando do Set-LabelPolicy para alterar o **OutlookDefaultlabel** para **Nenhum** em {OutlookDefaultLabel="None"}.

Executar: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Para obter mais informações sobre as etiquetas predefin Outlook, consulte Definir uma etiqueta [predefinida diferente para Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).