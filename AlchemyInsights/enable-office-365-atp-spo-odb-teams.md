---
title: Ativar o Office 365 ATP para equipas SharePoint, OneDrive e Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703437"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ativar o Office 365 Advanced Threat Protection for SharePoint Online, OneDrive e Microsoft Teams

1. Vá https://protection.office.com e inscreva-se.
2. Escolha**anexos seguros**de**política** > de gestão de **ameaças.** > 
3. Selecione **ligar ATP para As equipas SharePoint, OneDrive e Microsoft**e, em seguida, clique em **Guardar**.
4. (Recomendado) Como administrador global ou administrador do SharePoint Online, execute o [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DesdefinidoInizadoFileDownload** definido como *verdadeiro*.
5. (Recomendado) [Configurar alertas](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para ficheiros detetados.

> [!NOTE]
> O ATP irá analisar todos os ficheiros do SharePoint Online, OneDrive ou Microsoft Teams. Os ficheiros são digitalizados assincronicamente, através de um processo que utiliza eventos de partilha e atividade de hóspedes, juntamente com heurística inteligente e sinais de ameaça para identificar ficheiros maliciosos. Consulte [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).