---
title: Criar um site no SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052480"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar sites SharePoint usando modelos

Os modelos do site SharePoint são definições pré-construídas projetadas em torno de uma determinada necessidade de negócios. Para mais informações, veja [usando modelos para criar diferentes tipos de sites sharepoint.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Aqui estão alguns problemas/soluções comuns sobre salvar um site ou lista como um modelo no Sharepoint Online. 

**Salvar o botão de modelo do site/lista não está disponível ou ausente**

Os administradores precisarão permitir o script personalizado para ativar os recursos do modelo. Para etapas detalhadas, exemplos e considerações 

- [Permitir ou prevenir script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- O site Save como comando de modelo não é suportado e pode causar problemas em sites que usam a infraestrutura de publicação de servidores sharepoint.

**O modelo do site não pode ser criado ou não funciona corretamente**

O modelo pode estar faltando um [recurso](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado. Se o recurso não estiver disponível para ativar na coleção do site atual, você não pode usar o modelo do site para criar um site.

- Verifique se há listas ou bibliotecas excedendo o limite de visualização de [lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5.000 itens, pois isso pode bloquear a criação de um modelo do site.

- O site pode estar usando muitos recursos e, portanto, o modelo do site excede o limite de 50 MB.


- Há problemas para exibir dados de uma lista que usa uma coluna de pesquisa. Para obter mais informações, consulte a [lista gerada pelo Modelo não exibir dados da lista de pesquisa correta no SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Para obter informações mais detalhadas sobre problemas e soluções comuns, verifique [criar e usar modelos](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)do site.



