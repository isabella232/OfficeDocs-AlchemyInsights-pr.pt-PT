---
title: Problemas de desempenho no SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093778"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive Lenta, Inacessível ou Indisponível para Múltiplos Utilizadores

Se um OneDrive site do SharePoint ou um site do SharePoint não estiver disponível para múltiplos utilizadores que tinham acesso anteriormente, poderá haver um problema de serviço temporário. [Verifique o dashboard do estado de vida do serviço.](https://portal.office.com/adminportal/home#/servicehealth)

**Adicionar e licenciar o utilizador**

Certifique-se [de que atribui licenças aos utilizadores do Microsoft 365 para empresas.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Atribuir Permissões**

Se lhe tiver sido atribuída uma licença do SharePoint e ainda estiver a [](https://docs.microsoft.com/sharepoint/understanding-permission-levels) receber uma mensagem de acesso negado, certifique-se de que tem o nível de permissão adequado atribuído.

**Considere utilizar a funcionalidade de pedido de acesso**

A [funcionalidade de pedido de](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) acesso permite às pessoas pedir acesso a conteúdo que, de momento, não têm permissão para ver.

**Permitir scripts personalizados pode causar problemas de acesso negado**

Existem alguns cenários em que *a funcionalidade* Permitir script personalizado pode estar a apresentar um acesso negado. Para uma lista de funcionalidades afetadas, considerações de segurança e a capacidade de desativar a funcionalidade. Visite [Permitir ou impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

