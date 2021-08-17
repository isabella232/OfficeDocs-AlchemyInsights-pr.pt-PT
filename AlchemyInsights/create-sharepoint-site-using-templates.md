---
title: Criar um site no SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057977"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar sites do SharePoint através de modelos

A capacidade de guardar um site como um modelo não é suportada com Comunicação moderna ou Sites de Equipa. Para obter mais informações sobre como utilizar modelos, consulte o artigo [Guardar, transferir e carregar um site do SharePoint como um modelo](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Eis alguns problemas comuns/soluções sobre Guardar um Site ou Uma Lista como um modelo no SharePoint Online. 

**O botão Guardar modelo de site/lista não está disponível ou em falta**

Os administradores terão de Permitir o Script Personalizado para ativar as funcionalidades de modelo. Para obter passos detalhados, exemplos e considerações, consulte 

- [Permitir ou impedir um script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- O comando Guardar site como modelo não é suportado e pode causar problemas em sites que utilizem a Infraestrutura de Publicação do SharePoint Server.

**O modelo de site não pode ser criado ou não funciona corretamente**

O modelo poderá estar em falta uma [funcionalidade e](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) não será ativado. Se a funcionalidade não estiver disponível para ser ativada na coleção de sites atual, não pode utilizar o modelo de site para criar um site.

- Verifique se as listas ou bibliotecas excedem o [Limiar do Limite da Vista de Lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, pois pode bloquear a criação de um modelo de site.

- O site poderá estar a utilizar muitos recursos e, por isso, o modelo de site excede o limite de 50 MB.


- Existem problemas ao apresentar dados da lista que utiliza uma coluna de pesquisa. Para obter mais informações, consulte [A lista gerada pelo modelo não apresenta dados da lista de pesquisa correta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Para obter informações mais detalhadas sobre problemas e soluções comuns, consulte [Criar e utilizar modelos de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



