---
title: Atualizar os servidores de nomes do seu domínio para apontar para a Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: d9d66e366db14840a86b681deba78b89ddff5e068a3b931c88e493d2ec791b10
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073611"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Atualizar os servidores de nomes do seu domínio para apontar para a Microsoft

Nota: as alterações aos servidores de nomes podem, por vezes, demorar até 48 horas a serem propagadas.
  
Para configurar o seu domínio com a Microsoft, os servidores de nomes na sua registrora têm de ser atualizados. Crie ou edite os registos do seu servidor de nomes na sua entidade de registo de domínios.
  
1. Aceda ao site da sua entidade de registo de domínios e procure a área onde pode editar os servidores de nomes.

2. Crie ou edite dois registos de servidor de nomes de forma a que correspondam a estes valores:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Guarde as alterações.

Também pode encontrar instruções detalhadas neste artigo: Alterar servidores de nomes para configurar [servidores de Microsoft 365 com qualquer pessoa de registo de domínios](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  