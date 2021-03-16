---
title: Remova o serviço de fundo para a Pesquisa do Microsoft em Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816334"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Remova o serviço de fundo para a Pesquisa do Microsoft em Bing

Para remover o serviço de fundo para a Pesquisa do Microsoft em Bing, pode experimentar os seguintes remédios:

1. Para reverter para as definições originais do motor de busca, faça as seguintes coisas:

    a. Mude o **Use Bing como o seu motor de busca predefinido [para desligar](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.

    b. [Vá ao centro de administração microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) e limpe a definição que afeta todos os utilizadores da sua organização.

2. Para remover o serviço de fundo de um dispositivo individual, faça as seguintes tarefas:

    a. Escolha **o Painel de Controlo > programas > programas e funcionalidades**.

    b. Clique com o botão direito **Google in Bing** na lista de programas instalados e, em seguida, clique em **Desinstalar**.

3. Para remover o serviço de fundo de vários dispositivos na sua organização, faça login como administrador e execute o seguinte comando num script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
