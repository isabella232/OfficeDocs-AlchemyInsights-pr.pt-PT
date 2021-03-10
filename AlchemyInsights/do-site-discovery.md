---
title: Fazer descoberta do site
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694561"
---
# <a name="do-site-discovery"></a>Fazer descoberta do site

Se a sua organização ainda usa aplicações web antigas e planeia usar o modo Internet Explorer (o que a maioria dos clientes usa), então deve fazer alguma descoberta adicional do site.

**Já implementou uma versão mais antiga do Microsoft Edge**

Se já configuraste a tua Lista de Sites da Empresa para trabalhares para a versão antiga do Microsoft Edge, então a descoberta do teu site está quase pronta. A única coisa que talvez precises de fazer é adicionar sítios neutros.

Os locais neutros são normalmente sites que fornecem um único sinal de inscrição (SSO). Se for a um site neutro do Microsoft Edge, então pretende ficar no Microsoft Edge para autenticar. Se for a um site neutro no modo Internet Explorer, então deseja permanecer no modo Internet Explorer para autenticar.

Identifique quaisquer SSO ou outros sites neutros que utilize e adicione-os à sua Lista de Site Empresarial.

**O Internet Explorer é o seu navegador padrão**

Se você só está usando o Internet Explorer agora, você pode não saber quais sites atualizaram para padrões web modernos e que ainda requerem Internet Explorer. Você vai querer encontrar e adicionar estes sites à Lista de Sites da Empresa para que possa usar o modo Internet Explorer apenas para esses sites.

> [!NOTE]
> [Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) descobre sites que podem necessitar do modo Internet Explorer. Pode recolher dados em computadores que executam o Windows Internet Explorer 8 através do Internet Explorer 11 no Windows 10, Windows 8.1 ou Windows 7.

**Analisar os dados**

Depois de recolher os dados do site, recomendamos o seguinte processo de quatro etapas para analisar os dados:
1. Ordenar os dados por domínio e, em seguida, por URL.
2. Defina os limites de uma aplicação para configurar para o modo Internet Explorer. Pretende incluir todos os sites e controlos web que definem a aplicação, mas não quer incluir sites e controlos extras. Alguns sites podem ser tão simples como *https://contoso.com/app1* outros podem exigir que você defina vários sites e páginas.
3. Teste a aplicação para verificar se não funciona de forma nativa. Muitos sites oferecem conteúdo moderno quando detetam um navegador moderno e só oferecem conteúdo legado quando detetam o Internet Explorer.
4. Adicione a aplicação à sua Lista de Sites da Empresa se falhar no teste.

> [!NOTE]
> Como uma boa prática, agrupem todos os sites que compõem uma aplicação. Desta forma, quando atualiza uma aplicação, é mais fácil remover todo o site do modo Internet Explorer e começar a usar um navegador moderno para essa aplicação.

Assim que terminar a descoberta do site e analisar os dados, está pronto para começar a olhar para a sua estratégia de canal.

