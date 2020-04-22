---
title: Trabalhar com aplicações iOS VPP Regra Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719968"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhar com aplicações iOS VPP

Leia [como gerir as aplicações iOS adquiridas através de um programa de compra de volume com](https://docs.microsoft.com/intune/vpp-apps-ios) o Microsoft Intune para aprender sobre funcionalidades, constrangimentos e passos para fazer uso do Programa de Compra de Volume apple e o suporte para o mesmo no Microsoft Intune.
  
 **Questões Comuns:** "Atribuí uma aplicação iOS VPP aos meus utilizadores, mas a instalação falhou."
  
- Isto pode acontecer se um único token VPP for usado em vários fornecedores de gestão de dispositivos móveis. Os tokens VPP da Apple só podem ser usados com um fornecedor. Se usou um símbolo VPP com vários fornecedores, tem de voltar a carregar o token para Intune.

- A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para ver um relatório de utilização das suas licenças, vá à página de **licenças** de \> **aplicações Intune Mobile.** Para aprender a recuperar licenças em uso, consulte [este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
