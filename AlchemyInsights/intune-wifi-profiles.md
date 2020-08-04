---
title: Perfis Wi-Fi intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555317"
---
# <a name="intune-wi-fi-profiles"></a>Perfis Wi-Fi intune

A implementação bem sucedida da conectividade Wi-Fi para clientes MDM depende de um perfil corretamente implantado que reflita os requisitos da infraestrutura Wi-Fi corporativa. Para rever as definições apropriadas para as plataformas de clientes que está a investigar, consulte: 

[Adicione definições de Wi-Fi para dispositivos que executam o Android no Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Adicione definições de Wi-Fi para dispositivos dedicados e totalmente geridos do Android Enterprise no Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Adicione definições wi-fi para dispositivos iOS e iPadOS no Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Adicione definições de Wi-Fi para windows 10 e dispositivos posteriores no Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importar definições de Wi-Fi para dispositivos Windows em Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Questões Comuns**

**Estou a implantar um perfil Wi-Fi que depende de um certificado implantado especificado no perfil Wi-Fi. No entanto, os perfis de configuração mostram um estado de erro.**

Verifique se o seu dispositivo recebeu o certificado.

1. No Intune, vá a **todos os dispositivos** e selecione o dispositivo > **configuração do dispositivo**.

2. Verifique se todos os perfis esperados estão listados e em estado de sucesso.

3. Para um perfil Android, se tiver certificados intermédios na sua cadeia de certificados, certifique-se de que são implantados em dispositivos Android.

    Para verificar o estado do certificado, aceda aos perfis **de configuração do Dispositivo**Android intermediate  >  **Profiles**  >  **CA**  >  **Properties**  >  **Trusted Certificate**.

Se continuar a ver erros, reveja os procedimentos e as secções de resolução de problemas. Para obter mais informações, consulte [a Visão Geral para resolver os perfis de certificados SCEP com o Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Desloquei um perfil Wi-Fi para um dispositivo. A Intune está a mostrar que foi bem sucedida, mas o dispositivo não está a ligar-se ao Wi-Fi.**

Um estado de sucesso significa que a Intune implementou o perfil com sucesso como configurado. No entanto, estas configurações podem não corresponder aos seus requisitos de rede e/ou autenticação. Para obter mais detalhes sobre a tentativa de ligação, reveja os registos na infraestrutura e no serviço de autenticação (no controlador de ponto de acesso Wi-Fi e no servidor NPS/Radius). Você pode ter que trabalhar com a sua equipa de infraestrutura de rede, ou o fornecedor de Wi-Fi de terceiros, para recolher e rever registos.