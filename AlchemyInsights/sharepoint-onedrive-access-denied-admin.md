---
title: Remoção de mensagens do Access Negado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085239"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Remoção de mensagens do Access Negadas no SharePoint/OneDrive Centro de Administração

Se estiver a receber uma mensagem de acesso negado ao tentar navegar para um Centro de Administração do SharePoint/OneDrive, certifique-se de que atribui uma licença ao [utilizador.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Se o utilizador tiver uma licença, também [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) deverá certificar-se de que lhe é atribuída uma função de administrador que pode aceder aos centros de administração.

Este problema também pode ocorrer quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN). A nova conta é criada utilizando um valor PUID (Passaporte Exclusivo ID) diferente. Quando o utilizador tenta aceder a uma coleção de site ou à sua OneDrive, o utilizador tem um PUID incorreto. Um segundo cenário envolve a sincronização de diretórios com uma unidade organizacional do Active Directory (OU). Se os utilizadores já têm a sua primeira ação e, em seguida, foram movidos para um OU diferente e voltarem a silhá-lo com o SharePoint, poderão detetá-lo.

Para resolver este problema, deve restaurar o UPN original com os passos no artigo [Restaurar um utilizador no Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Nota: Se um OneDrive de Administração do SharePoint ou um Administrador do SharePoint não estiver disponível para múltiplos utilizadores que tinham acesso anteriormente, poderá haver um problema de serviço temporário.  [Verifique o dashboard do estado de vida do serviço.](https://portal.office.com/adminportal/home#/servicehealth)


