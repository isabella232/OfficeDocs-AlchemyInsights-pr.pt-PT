---
title: Usando perfis de e-mail com Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555248"
---
# <a name="using-email-profiles-with-intune"></a>Usando perfis de e-mail com Intune

O Intune pode ser usado para criar e implementar perfis de e-mail para o cliente de e-mail nativo (incorporado) em várias plataformas de dispositivos.

Para obter informações sobre algumas das restrições associadas aos perfis de e-mail, incluindo a forma como a presença de perfis existentes são tratados e como remover perfis de e-mail, consulte adicionar definições de [e-mail a dispositivos que utilizem o Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Para obter mais informações sobre como criar perfis de e-mail para cada plataforma do dispositivo, consulte:

[Configurações de dispositivos Android para configurar e-mail, autenticação e sincronização no Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Adicione as definições de e-mail para dispositivos iOS e iPadOS no Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Definições de perfil de e-mail no Microsoft Intune para dispositivos que executam o Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Definições de perfil de e-mail para dispositivos que executam o Windows 10 no Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Questão comum de sincronização**

**Um PERFIL KNOX no Android impede que os Contactos, Calendário e Tarefas dos utilizadores sejam sincronizados com dispositivos do utilizador.**

O perfil de e-mail KNOX do Android KNOX oferece ao administrador a opção de decidir quais os tipos de conteúdo sincronizados com o dispositivo, definindo cada um para ativar.

Se a definição de qualquer um dos tipos de conteúdo estiver definida como **Não configurada** (o padrão), esse tipo de conteúdo não é sincronizado automaticamente. Um utilizador pode ativar o tipo de conteúdo que pretende diretamente no dispositivo manualmente, mas essa configuração é substituída pela definição de política Intune, e a sincronização para para esse tipo de conteúdo.

