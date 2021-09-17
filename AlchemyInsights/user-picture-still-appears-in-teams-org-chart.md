---
title: A imagem de utilizador continua a aparecer no Microsoft Teams organização
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422322"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>A imagem de utilizador continua a aparecer no Microsoft Teams organização

Se uma ou mais pessoas na sua organização foram desativadas ou removidas e a respetiva fotografia de perfil continuar a aparecer no organization chart, é possível que a definição **ShowInAddressLists** esteja definida como Falso: 

1. Vá para o centro de administração do Microsoft 365 > [Utilizadores Ativos](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) e selecione o utilizador com a fotografia que ainda aparece. 
1. Selecione **o separador** Correio e certifique-se de que a opção Mostrar **na lista de endereços global** está definida como **Não.**

Se definir **ShowInAddressLists** para **Não** não funcionar, verifique o seguinte: 

- O utilizador poderá ser apresentado a partir da lista de destinatários no Exchange. Para mais informações, consulte Gerir [listas de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- O utilizador poderá ser apresentado a partir da lista de endereços no Azure Active Directory. Para mais informações, consulte [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 