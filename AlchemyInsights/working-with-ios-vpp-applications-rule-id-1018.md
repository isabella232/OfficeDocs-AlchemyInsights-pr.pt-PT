---
title: Trabalhar com aplicações iOS VPP Regra Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688957"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhar com aplicações iOS VPP

Leia [Como gerir as aplicações iOS adquiridas através de um programa de compra de volume com o Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para aprender sobre funcionalidades, constrangimentos e passos para utilizar o Apple Volume Purchase Program e o suporte para o mesmo no Microsoft Intune.
  
 **Questões comuns:** "Atribuí uma aplicação de VPP iOS aos meus utilizadores, mas a instalação falhou."
  
- Isto pode acontecer se um único token VPP for usado em vários fornecedores de gestão de dispositivos móveis. Os tokens VPP da Apple só podem ser usados com um fornecedor. Se usou um token VPP com vários fornecedores, deve re-carregar o token para Intune.

- A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para ver um relatório de utilização das suas licenças, aceda à página de licenças da Aplicação de **aplicações Intune Mobile.** \> **App licenses** Para aprender a recuperar licenças em uso, consulte [este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
