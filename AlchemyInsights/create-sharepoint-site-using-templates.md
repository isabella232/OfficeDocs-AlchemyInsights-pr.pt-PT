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
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770434"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar sites sharePoint usando modelos

A capacidade de salvar um site como modelo não é suportada com sites modernos de Comunicação ou Equipa. Para obter mais informações sobre a utilização de modelos, consulte [Guardar, transferir e carregar um site do SharePoint como modelo](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Aqui estão algumas questões/soluções comuns no que diz respeito a salvar um site ou lista como um modelo no Sharepoint Online. 

**Salvar o botão de modelo de site/lista não está disponível ou em falta**

Os administradores terão de permitir o Script Personalizado para ativar as funcionalidades do modelo. Para passos detalhados, exemplos e considerações ver 

- [Permitir ou prevenir scriptpersonalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- O site Save como comando de modelo não é suportado e pode causar problemas em sites que usam a Infraestrutura de Publicação do Servidor SharePoint.

**O modelo do site não pode ser criado ou não funciona corretamente**

O modelo pode estar a faltar uma [funcionalidade](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não ativa. Se a funcionalidade não estiver disponível para ser ativada na coleção atual do site, não pode utilizar o modelo do site para criar um site.

- Verifique se alguma lista ou biblioteca excede o limite de limite de 5000 itens da [lista,](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) pois isso pode bloquear a criação de um modelo de site.

- O site pode estar a usar demasiados recursos e, portanto, o modelo do site excede o limite de 50 MB.


- Existem problemas em apresentar dados de uma lista que usa uma coluna de procuração. Para mais informações, consulte a [lista gerada pelo Modelo não apresentar dados da lista de pesquisas corretas no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Para obter informações mais detalhadas sobre problemas e soluções comuns, verifique [criar e utilizar modelos](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)de site .



