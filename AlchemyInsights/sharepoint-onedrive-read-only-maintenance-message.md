---
title: 127 obter um erro de TenantAccessBlockedException quando aceder a correio electrónico?
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5613138e7613deb264a7ab2c966f8b9c4a24763d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736413"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Só de leitura para mensagens de manutenção ao tentar utilizar o SharePoint ou OneDrive

Os utilizadores poderão receber uma só de leitura para mensagens de manutenção quando tenta utilizar o SharePoint ou OneDrive.

Verifique se existe manutenção activa que ocorram no seu tenant navegando para o [Centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter). Finalmente, certifique-se de que visitar a página de[Estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar a existência de quaisquer avisos/incidentes que pode estar a ocorrer.

Se nem o Centro de mensagens ou o serviço de saúde Dashboard tiver anotado nada sobre trabalhos correntes de manutenção para o locatário, isto pode ser um problema de cache de browser.

Tente limpar a cache do browser antes de navegar para o site.

- No browser do Microsoft Edge, vá para definições de mais

- Em navegação clara, seleccione Escolher o que para a desmarcar.
- Seleccione os Cookies e a caixa de verificação de dados do Web site guardado e seleccione Limpar.

**Nota**: estes passos podem ser diferentes quando utiliza outros browsers, tais como o Firefox ou o cromado.

