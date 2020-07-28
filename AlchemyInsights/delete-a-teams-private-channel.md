---
title: Excluir um canal privado das Equipas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439918"
---
# <a name="delete-a-teams-private-channel"></a>Excluir um canal privado das Equipas

A Microsoft está ciente de um problema que elimina um canal privado do Teams se tiver políticas de retenção sharePoint ativadas para o site SharePoint subjacente. A Microsoft está a trabalhar numa correção. Entretanto, pode utilizar as seguintes soluções para eliminar o canal privado.

**Excluir a recolha team/site da política de retenção de Sharepoint.**

1. Vá ao portal de administração do Office 365 e selecione **Mostrar tudo** no painel de navegação à esquerda.
2. Nos **centros de administração,** vá para a Política de Prevenção de Perda de Dados de Conformidade & De **Segurança**  >  **Data Loss Prevention**  >  **Policy**.
3. Identifique qualquer política que se aplique aos sites sharepoint e modifique a política para que o site sharepoint para a equipa que contenha o canal privado NÃO seja incluído na política de retenção.
4. Salve a apólice.
    Pode levar até 24 horas para que as definições de política produzam efeitos.
    Depois de o site ter sido excluído, pode apagar o canal privado.  
    
Poderá ***might*** eliminar o canal privado utilizando o Microsoft Teams no seu dispositivo Android. 

Para obter informações relacionadas com o SharePoint, consulte [Não conseguir eliminar itens no SharePoint Online ou no OneDrive para negócios.](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)