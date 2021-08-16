---
title: Deteção de site
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030769"
---
# <a name="do-site-discovery"></a>Deteção de site

Se a sua organização ainda utilizar aplicações Web legadas e planos para utilizar o modo Internet Explorer (que a maioria dos clientes faz), deve fazer alguma deteção adicional de sites.

**Já implementou uma versão anterior do Microsoft Edge**

Se já tiver configurado a Lista de Site de Empresa para funcionar na versão legada do Microsoft Edge, a deteção do site está quase a terminar. A única coisa que poderá ter de fazer é adicionar sites neutros.

Normalmente, os sites neutros são sites que fornecem o primeiro sinal (SSO). Se for a um site neutro a partir Microsoft Edge, então pretende manter-se Microsoft Edge autenticar. Se for a um site neutro no modo Internet Explorer, pretende manter-se no modo Internet Explorer para autenticar.

Identifique quaisquer SSOs ou outros sites neutros que utilize e adicione-os à Sua Lista de Sites de Empresa.

**O Internet Explorer é o seu browser predefinido**

Se agora só estiver a utilizar o Internet Explorer, poderá não saber quais os sites que atualizaram para padrões Web modernos e que ainda necessitam do Internet Explorer. Poderá querer encontrar e adicionar estes sites à Lista de Sites de Empresa para poder utilizar o modo do Internet Explorer apenas para esses sites.

> [!NOTE]
> [A Deteção de](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) Sites de Empresa deteta sites que poderão necessitar do modo Internet Explorer. Pode recolher dados em computadores que executam o Windows Internet Explorer 8 até ao Internet Explorer 11 no Windows 10, Windows 8.1 ou Windows 7.

**Analisar os dados**

Após recolher os dados do site, recomendamos o seguinte processo de quatro passos para analisar os dados:
1. Ordenar os dados por domínio e, em seguida, por URL.
2. Defina os limites de uma aplicação para configurar para o modo Internet Explorer. Pretende incluir todos os sites e controlos Web que definem a aplicação, mas não quer incluir sites e controlos extra. Alguns sites podem ser tão simples como outros, enquanto outros podem exigir que *https://contoso.com/app1* defina múltiplos sites e páginas.
3. Teste a aplicação para verificar se não funciona nativamente. Muitos sites irão oferecer conteúdos modernos quando detetarem um browser moderno e oferecerem apenas conteúdos legados quando detetarem o Internet Explorer.
4. Adicione a aplicação à Sua Lista de Site de Empresa se o teste falhar.

> [!NOTE]
> Como prática recomendada, agrupe todos os sites que constituem uma aplicação. Desta forma, quando atualiza uma aplicação, é mais fácil remover todo o site do modo Internet Explorer e começar a utilizar um browser moderno para essa aplicação.

Quando terminar a deteção de site e analisar os dados, está pronto para começar a analisar a sua estratégia de canal.

