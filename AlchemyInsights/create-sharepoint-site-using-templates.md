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
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732246"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar sites sharePoint usando modelos

A capacidade de salvar um site como modelo não é suportada com comunicações modernas ou sites de equipa. Para obter mais informações sobre a utilização de modelos [consulte Guardar, transferir e carregar um site do SharePoint como modelo.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

Aqui estão algumas questões/soluções comuns sobre guardar um site ou lista como um modelo no Sharepoint Online. 

**O botão de modelo de site/lista não está disponível ou em falta**

Os administradores terão de permitir o Script Personalizado para ativar as funcionalidades do modelo. Para passos, exemplos e considerações detalhadas ver 

- [Permitir ou prevenir script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- O site Save como comando de modelo não é suportado e pode causar problemas em sites que usam a Infraestrutura de Publicação do Servidor SharePoint.

**O modelo do site não pode ser criado ou não funciona corretamente**

O modelo pode estar a perder uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado. Se a funcionalidade não estiver disponível para ser ativada na recolha atual do site, não poderá utilizar o modelo do site para criar um site.

- Verifique se alguma lista ou biblioteca excede o limiar limite de [visualização](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de lista de 5000 itens, uma vez que isso pode bloquear a criação de um modelo de site.

- O site pode estar a usar demasiados recursos e, portanto, o modelo do site excede o limite de 50 MB.


- Existem problemas em apresentar dados de uma lista que utiliza uma coluna de procuração. Para obter mais informações, consulte [a lista gerada por Modelos não exibe dados da lista de pesquisa correta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Para obter informações mais detalhadas sobre problemas e soluções comuns, verifique [criar e utilizar modelos do site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



