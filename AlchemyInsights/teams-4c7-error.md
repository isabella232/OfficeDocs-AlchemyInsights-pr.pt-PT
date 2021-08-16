---
title: Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049319"
---
# <a name="4c7-error-in-microsoft-teams"></a>Erro 4c7 em Microsoft Teams

Este erro ocorre porque o Microsoft Teams aUtenticação de Formulários. Quando implementa os Serviços de Federação do Active Directory (AD FS), a Autenticação de Formulários não está ativada para a intranet por predefinição. Se Windows Autenticação Integrada falhar, ser-lhe-á pedido para o fazer através da Autenticação de Formulários.

Para resolver este problema, ative a Autenticação de Formulários utilizando o snap-in da Consola de Gestão da Microsoft (MMC) do AD FS no computador que tem a cópia local do Active Directory. Para tal, siga estes passos: 

1. No painel de navegação, navegue até Políticas de **Autenticação.**
2. Em **Ações** no painel de detalhes, selecione **Editar Autenticação Principal Global.**
3. No separador **Intranet,** selecione **Autenticação de Formulários**.
4. **Selecione OK** (ou **Aplicar**).