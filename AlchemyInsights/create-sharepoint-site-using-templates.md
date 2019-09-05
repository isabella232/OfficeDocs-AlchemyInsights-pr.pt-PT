---
title: Criar um site SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755319"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar sites do SharePoint utilizando modelos

Modelos de site do SharePoint são definições previamente concebidas destinadas em torno de uma determinada necessidade da empresa. Para mais informações, consulte [utilizar modelos para criar diferentes tipos de sites do SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Eis algumas questões/soluções comuns relativas ao guardar um Site ou lista como um modelo no Sharepoint Online. 

**Botão de modelo de site/lista de guardar não está disponível ou em falta**

Os administradores serão necessário permitir Script personalizado para activar as funcionalidades do modelo. Para obter informações detalhadas, consulte os exemplos e considerações 

- [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- O site de guardar como comando de modelo não é suportado e pode causar problemas em sites que utilizem a infra-estrutura de publicação do SharePoint Server.

**O modelo de site não é possível criar ou não funciona correctamente**

O modelo pode estar em falta uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não vai activar. Se a funcionalidade não está disponível para activar a colecção de sites actual, é possível utilizar o modelo de site para criar um site.

- Verifique se todas as listas ou bibliotecas de excederem o [Limiar de limite de vista de lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, como este pode bloquear a criação de um modelo de site.

- O site poderá estar a utilizar demasiados recursos e, por conseguinte, o modelo de site excede o limite de 50 MB.


- Existem problemas em visualizar dados de uma lista que utiliza uma coluna de pesquisa. Para mais informações, consulte a [lista gerada de modelo não apresenta os dados na lista de pesquisa correcta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Para obter informações mais detalhadas sobre problemas e soluções comuns, consulte [criar e utilizar modelos de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



