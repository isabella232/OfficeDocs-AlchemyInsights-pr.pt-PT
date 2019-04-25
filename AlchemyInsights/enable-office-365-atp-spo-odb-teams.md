---
title: Activar ATP do Office 365 para SharePoint, OneDrive e equipas da Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403044"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activar a protecção do Office 365 ameaça avançadas para SharePoint Online, OneDrive e equipas da Microsoft

1. Vá para https://protection.office.com e iniciar sessão.
2. Escolher **Gestão ameaças** > **política** > **Anexos seguros**.
3. Seleccione **Activar ATP para SharePoint, OneDrive e equipas da Microsoft**e, em seguida, clique em **Guardar**.
4. (Recomendado) Como um administrador global ou um administrador do SharePoint Online, execute o cmdlet [Conjunto SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *true*.
5. (Recomendado) [Configurar alertas](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para ficheiros detectados.

> [!NOTE]
> ATP será nPara pesquisa todos os ficheiros só no Online do SharePoint, OneDrive ou Teams da Microsoft. Ficheiros são analisados de forma assíncrona, através de um processo que utiliza eventos de actividade de partilha e de convidado, bem como heurística avançada e sinais de ameaça para identificar ficheiros maliciosos. Consulte [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).