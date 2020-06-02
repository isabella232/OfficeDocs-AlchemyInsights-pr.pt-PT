---
title: Ativar o Office 365 ATP para as equipas SharePoint, OneDrive e Microsoft
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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506929"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ativar o Office 365 Advanced Threat Protection for SharePoint Online, OneDrive e Microsoft Teams

1. Vá https://protection.office.com e inscreva-se.
2. Escolha **Threat management**os  >  **Policy**  >  **anexos seguros da**política de gestão de ameaças .
3. Selecione **Ligue ATP para SharePoint, OneDrive e Microsoft Teams**e, em seguida, clique em **Guardar**.
4. (Recomendado) Como administrador global ou administrador on-line sharePoint, executar o [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *verdadeiro*.
5. (Recomendado) [Configurar alertas](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para ficheiros detetados.

> [!NOTE]
> O ATP irá analisar todos os ficheiros do SharePoint Online, OneDrive ou Microsoft Teams. Os ficheiros são digitalizados assíncrono, através de um processo que utiliza eventos de partilha e atividade de hóspedes, juntamente com heurística inteligente e sinais de ameaça para identificar ficheiros maliciosos. Ver [ATP para SharePoint, OneDrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).