---
title: A imagem do utilizador não é mostrada Microsoft Teams organization chart
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792882"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>A imagem do utilizador não é mostrada Microsoft Teams organization chart

Se uma ou mais pessoas na sua organização não encontrarem a respetiva fotografia de perfil no organization chart, é possível que a definição **ShowInAddressLists** seja definida como **Falso:**

1. Vá para o centro de administração do Microsoft 365 > [**Utilizadores Ativos**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)e selecione o utilizador com a fotografia em falta. 
1. Selecione **o separador** Correio e certifique-se de que a opção Mostrar **na lista de endereços global** está definida como **Sim.** 

Se a **definição MostrarInAddressLists** **para Sim** não funcionar, verifique o seguinte:

- O utilizador pode estar oculto da lista de destinatários no Exchange. Para mais informações, consulte Gerir [listas de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- O utilizador poderá estar oculto da lista de endereços no Azure Active Directory. Para mais informações, consulte [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
