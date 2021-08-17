---
title: Trabalhar com o ID de Regra de Aplicações do VPP do iOS 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083025"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhar com Aplicações VPP do iOS

Leia Como gerir [aplicações iOS](https://docs.microsoft.com/intune/vpp-apps-ios) compradas através de um programa de compra em volume com o Microsoft Intune para saber mais sobre funcionalidades, restrições e passos para utilizar o Programa de Compra em Volume da Apple e o suporte para o mesmo no Microsoft Intune.
  
 **Problemas Comuns:** "Assinei uma aplicação VPP do iOS aos meus utilizadores, mas a instalação falhou."
  
- Isto pode acontecer se um único token VPP for utilizado em múltiplos fornecedores de gestão de dispositivos móveis. Os tokens VPP da Apple só podem ser utilizados com um fornecedor. Se tiver utilizado um token VPP com vários fornecedores, tem de carregar o token para o Intune.

- A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para ver um relatório de utilização das suas licenças, vá para a página de licenças da Aplicação **Intune** \>  Mobile. Para saber como recuperar licenças em utilização, consulte [este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
