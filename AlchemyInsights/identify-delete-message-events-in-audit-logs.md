---
title: Identificar Eliminar mensagem eventos nos registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755163"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Registos de auditoria para mensagens de correio electrónico eliminados

A partir de Janeiro de 2019, Microsoft é a activação por predefinição o registo de auditoria de caixa de correio. Caso contrário, para rever os eventos de mensagem de eliminação de um utilizador específico, tem de activar manualmente as acções de eliminação para auditoria. Se a caixa de correio de auditoria registo já está activado para a sua organização ou para o utilizador específico, siga os passos abaixo.

1. Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/)

2. Clique em **Procurar e de investigação** e seleccione a **Procura de registo de auditoria**.

3. Seleccione o intervalo de datas nos campos **data de início** e **data de fim** . Especificar o nome de utilizador que pretende investigar (o utilizador que os itens eliminados). No campo **actividades** , seleccione **as mensagens eliminadas da pasta Itens eliminados** e **Moved mensagens para a pasta Itens eliminados**.

4. Clique em **Procurar**.

Nos resultados, seleccione um registo de auditoria. Na lista de opções de detalhes, clique em **Mais informações**. Obter informações adicionais sobre a item eliminado (por exemplo, a linha de assunto e a localização do item quando foi eliminado) são apresentadas no campo **AffectedItems** . A propriedade **ClientInfoString** irá mostrar-se a eliminação ocorreu no Outlook, Outlook na web (anteriormente conhecido como o Outlook Web App) ou qualquer outro dispositivo.

Para mais informações, consulte [determinar que configurou para uma caixa de correio de reencaminhamento de correio electrónico](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Nota**: não é possível obter itens eliminados utilizando a funcionalidade de registo de auditoria. Para obter mensagens eliminadas no Outlook na web, consulte [recuperar itens no Outlook Web App eliminados](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
