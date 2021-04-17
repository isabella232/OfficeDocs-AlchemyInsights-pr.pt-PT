---
title: MC210173 — Descontinuação da nova funcionalidade de Formulários personalizados do SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831817"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 — Descontinuação da nova funcionalidade de Formulários personalizados do SharePoint Designer

Identificámos um problema que afeta a funcionalidade para [criar Formulários personalizados](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) do SharePoint Designer no SharePoint Online. Após examinar cuidadosamente, determinámos que não existe uma solução conhecida para este problema e decidimos desativar a funcionalidade de criação de Formulários personalizados a partir das 03:00 UTC de sábado, 25 de abril de 2020. Esta alteração não afeta a capacidade para editar Formulários criados anteriormente ou outras funcionalidades existentes no SharePoint Online Designer.

Após esta alteração ter sido efetuada, os utilizadores poderão ter recebido o seguinte erro ao criar novos Formulários: "Não foi possível guardar as alterações à lista no servidor".

Os utilizadores que tiraram partido do SharePoint Designer anteriormente para criar Formulários personalizados podem utilizar o [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) para esta finalidade.

O PowerApps é uma ferramenta avançada e fácil de utilizar que permite aos utilizadores a operar na experiência moderna do SharePoint Online criar e editar os Formulários personalizados das bibliotecas de documentos e listas do SharePoint a partir de uma janela do browser. O PowerApps não requer um conhecimento de codificação tradicional ou transferências de aplicações adicionais, como o InfoPath.

**Nota**: os utilizadores do SharePoint Online Clássico terão de mudar temporariamente para a experiência Moderna para aceder e utilizar o PowerApps. Porém, todos os Formulários personalizados criados no PowerApps são acessíveis pelos utilizadores da experiência Clássica do SharePoint Online.
