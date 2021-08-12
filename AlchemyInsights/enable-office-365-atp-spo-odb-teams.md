---
title: Ativar Office 365 ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964644"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ativar o Microsoft Defender Office 365 para SharePoint Online, OneDrive e Microsoft Teams

1. Vá para https://protection.office.com e inscreva-se.
2. **Selecionar Política de**  >    >  **Gestão de Cofre Anexos**.
3. **Selecione Acionar o Defender para Office 365 para SharePoint, OneDrive e Microsoft Teams e,** em seguida, clique em **Guardar**.
4. (Recomendado) Como administrador global ou administrador do SharePoint Online, execute o cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido para *true*.
5. (Recomendado) [Configurar alertas para ficheiros](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) detetados.

> [!NOTE]
> O Microsoft Defender Office 365 irá analisar todos os ficheiros no SharePoint Online, OneDrive ou Microsoft Teams. Os ficheiros são analisados assíncronamente através de um processo que utiliza eventos de partilha e de atividade de convidados, juntamente com sinais de heurística e ameaça inteligentes para identificar ficheiros maliciosos. Consulte [Microsoft Defender para Office 365 para SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).