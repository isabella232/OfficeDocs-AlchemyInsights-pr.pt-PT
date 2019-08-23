---
title: Trabalhar com iOS VPP aplicações regra Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558016"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhar com iOS VPP aplicações

Leia [como gerir aplicações de iOS adquiridas através de um programa de volume de compras com Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para obter informações sobre funcionalidades, restrições e passos para que utilize o programa de compras de Volume da Apple e o suporte para o mesmo no Microsoft Intune.
  
 **Problemas comuns:** "Que atribuí uma aplicação VPP iOS a meus utilizadores, mas falha na instalação."
  
- Isto pode acontecer se um token VPP único é utilizado através de vários fornecedores de gestão do dispositivo móvel. Os tokens VPP de Apple só podem ser utilizados com um fornecedor. Se utilizou um token VPP com vários fornecedores, tem de carregar novamente o token para Intune.

- A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para ver um relatório de utilização para as licenças, vá para o **apps Intune Mobile** \> página de **licenças de aplicação** . Para obter informações sobre como recuperar de licenças em utilização, consulte [deste artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
