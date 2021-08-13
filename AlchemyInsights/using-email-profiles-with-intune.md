---
title: Utilizar perfis de e-mail com o Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919434"
---
# <a name="using-email-profiles-with-intune"></a>Utilizar perfis de e-mail com o Intune

O Intune pode ser utilizado para criar e implementar perfis de e-mail para o cliente de e-mail nativo (incorporado) em várias plataformas de dispositivos.

Para informações sobre algumas das restrições associadas aos perfis de e-mail, incluindo como a presença de perfis existentes é tratada e como remover perfis de e-mail, consulte Adicionar definições de e-mail a dispositivos com o [Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Para mais informações sobre como criar perfis de e-mail para cada plataforma de dispositivo, consulte:

[Definições de dispositivo Android para configurar o e-mail, a autenticação e a sincronização no Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Adicionar definições de e-mail para dispositivos iOS e iPadOS no Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Definições de perfil de e-Microsoft Intune para dispositivos a executar o Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Definições de perfil de e-mail para dispositivos que executem Windows 10 no Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problema de syncing comum**

**Um perfil de e-mail KNOX no Android impede que os Contactos, Calendário e Tarefas do utilizador sincronizam com os dispositivos do utilizador.**

O perfil de e-mail KNOX para Android KNOX oferece ao administrador a opção de decidir quais os tipos de conteúdo que são sincronizados com o dispositivo ao definir cada um para ativado.

Se a definição para qualquer um dos tipos de conteúdo estiver definida como Não configurado **(a** predefinição), esse tipo de conteúdo não será sincronizado automaticamente. Um utilizador pode ativar o tipo de conteúdo que pretende diretamente no dispositivo manualmente, mas essa configuração é escrita manualmente pela definição da política do Intune e a sincronização para esse tipo de conteúdo.

