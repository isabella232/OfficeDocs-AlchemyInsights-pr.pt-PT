---
title: DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932669"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP pode precisar de um tipo personalizado

**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano. Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup. Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.

Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana. Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos. No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.

**DLP pode requerer um tipo de informação personalizada**

Com uma política de prevenção de perdas de dados (DLP), pode identificar e proteger dados sensíveis na sua organização. Em alguns cenários, poderá ser necessário criar o seu **próprio** tipo de informação personalizada e sensível para proteger os dados da sua organização.

Por exemplo, a sua organização pode precisar de identificar e proteger iDs ou outros dados de funcionários em algum formato específico do seu org. Em caso afirmativo, consulte os seguintes artigos para obter mais informações.
  
 **Personalize um tipo de informação sensível incorporada**
  
Se um tipo de informação sensível incorporado atender às suas necessidades com apenas alguns ajustes, pode [personalizar um tipo de informação sensível incorporado](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Por exemplo, pode adicionar ou remover palavras-chave, ou adicionar ou remover provas de apoio, como uma data ou endereço.
  
 **Criar um tipo de informação sensível personalizado**
  
Mas se precisar de identificar e proteger completamente um tipo diferente de informação sensível, pode criar um tipo de [informação sensível personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) na UI do Centro de Conformidade & Segurança.
  
**Criar um tipo de informação sensível personalizado em Security & Compliance Center PowerShell**

Finalmente, se o UI não fornecer todas as opções de que necessita, pode criar um tipo de [informação sensível personalizado em Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis.
