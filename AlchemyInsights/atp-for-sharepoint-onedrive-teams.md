---
title: ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715572"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP para SharePoint, OneDrive e Microsoft Teams

Siga estes passos para permitir a Proteção Avançada de Ameaças:

1. Vá [https://protection.office.com](https://protection.office.com) e inscreva-se com um administrador global ou conta de administrador de segurança.

2. No painel de navegação à **Policy** esquerda sob **gestão de ameaças,** escolha \> **Os Anexos Seguros de**Política .

3. Selecione **Ligue ATP para SharePoint, OneDrive e Microsoft Teams**.

4. [Crie uma política de alerta de atividade](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) para receber notificações quando detetarmos ficheiros maliciosos.

Para obter instruções completas, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)

**Nota:** Por design, o ATP não digitaliza todos os ficheiros do SharePoint Online, OneDrive for Business ou Microsoft Teams. Os ficheiros são analisados assíncrono por um processo que utiliza atividade de partilha, atividade de hóspedes e sinais de ameaça para identificar ficheiros maliciosos. Para mais informações, consulte este [tópico.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
