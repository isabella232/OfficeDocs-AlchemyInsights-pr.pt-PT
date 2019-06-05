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
ms.openlocfilehash: 54ebc269b391e6b0d607e55af8283ebf3d9e2aa7
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715082"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Só de leitura para mensagens de manutenção ao tentar utilizar o SharePoint ou OneDrive

Os utilizadores poderão receber uma só de leitura para mensagens de manutenção quando tenta utilizar o SharePoint ou OneDrive.

Verifique se existe manutenção activa que ocorram no seu tenant navegando para o <a href="https://portal.office.com/adminportal/home#/MessageCenter">Centro de mensagens</a>. Finalmente, certifique-se de que visitar a página de <a href="https://portal.office.com/adminportal/home#/servicehealth">Estado de funcionamento do serviço</a> para verificar a existência de quaisquer avisos/incidentes que pode estar a ocorrer.

Se nem o Centro de mensagens ou o serviço de saúde Dashboard tiver anotado nada sobre trabalhos correntes de manutenção para o locatário, isto pode ser um problema de cache de browser.

Tente limpar a cache do browser antes de navegar para o site.

  <li>No browser do Microsoft Edge, vá para <strong>mais &hellip; &gt; definições</strong></li>  <li>Em <strong>Navegação clara </strong>, seleccione <strong>Escolher o que para a desmarcar</strong>.</li>  <li>Seleccione os Cookies e a caixa de verificação de dados do Web site guardado e seleccione <strong>Limpar</strong>.</li>  </ol>  

**Nota**: estes passos podem ser diferentes quando utiliza outros browsers, tais como o Firefox ou o cromado.

