---
title: Desafine o Microsoft Edge como o navegador padrão num dispositivo macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491811"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Desafine o Microsoft Edge como o navegador padrão num dispositivo macOS

Utilize um destes dois métodos para definir o Microsoft Edge como o navegador padrão:

Método 1: Flash o dispositivo com uma imagem do macOS onde o Microsoft Edge já foi definido como o navegador padrão.

Método 2: Descreva a política DefaultBrowserSettingEnabled para solicitar ao utilizador que definisse o Microsoft Edge como o navegador predefinido.

Qualquer um dos métodos permite que um utilizador altere o navegador predefinido. Por esta razão, recomendamos que implemente a política DefaultBrowserSettingEnabled mesmo que tenha utilizado o método 1. Se um utilizador alterar o navegador predefinido após a implementação da política, a política solicita ao utilizador que reenrou o navegador predefinido ao Microsoft Edge.
