---
title: Criar um site SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515009"
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


- Existem problemas em visualizar dados de uma lista que utiliza uma coluna de pesquisa. Para mais informações, consulte a [lista gerada de modelo não apresenta os dados na lista de pesquisa correcta no SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Para obter informações mais detalhadas sobre problemas e soluções comuns, consulte [criar e utilizar modelos de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



