---
title: Listas grandes do SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767296"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Trabalhe com grandes listas e bibliotecas no SharePoint

As listas e bibliotecas do SharePoint podem conter até 30 milhões de itens, mas quando têm mais de 5.000 itens, poderá ver um erro de List View Threshold quando tentar trabalhar com eles. Este limiar está em vigor para manter o desempenho do serviço. Não pode ser alterado. Para evitar atingir este limiar:

**Use moderno**

As vistas que mostram muitos itens funcionam melhor na experiência moderna. [Use a experiência moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) para evitar erros que possa ver na experiência clássica.

**Adicionar índices**

Quando filtrar ou classificar por uma coluna que não tem um índice, pode ver uma mensagem de erro. [Adicione um índice](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manualmente a partir de **Definições** de lista no menu de definições, em seguida, **Colunas Indexadas**.

**Editar a vista da lista**

Se ocorrer um erro ao trabalhar com uma grande lista, [edite a sua visualização da lista](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

As quatro alterações seguintes eliminarão os erros de limiar da visualização da lista. Faça as quatro alterações para remover todos os erros. Se ainda estiver a ter erros, verifique [Gerir grandes listas e bibliotecas.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Selecione **Nenhum** de ambos **os primeiros classificados pela coluna** **e, em seguida, separe pela coluna**.
2. Selecione **Nenhum** de ambos **os primeiros grupos pela coluna** **e, em seguida, agrupe-se pela coluna**.
3. Selecione **Nenhuma** para todas as colunas da secção **Totals.**
4. Desmarque todas as colunas, menos uma, para visualização da secção **Colunas.**

