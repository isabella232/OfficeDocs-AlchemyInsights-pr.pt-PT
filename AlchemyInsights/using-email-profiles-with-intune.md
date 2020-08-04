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
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="03d63-102">Usando perfis de e-mail com Intune</span><span class="sxs-lookup"><span data-stu-id="03d63-102">Using email profiles with Intune</span></span>

<span data-ttu-id="03d63-103">O Intune pode ser usado para criar e implementar perfis de e-mail para o cliente de e-mail nativo (incorporado) em várias plataformas de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="03d63-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="03d63-104">Para obter informações sobre algumas das restrições associadas aos perfis de e-mail, incluindo a forma como a presença de perfis existentes são tratados e como remover perfis de e-mail, consulte adicionar definições de [e-mail a dispositivos que utilizem o Intune.](https://docs.microsoft.com/intune/email-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="03d63-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="03d63-105">Para obter mais informações sobre como criar perfis de e-mail para cada plataforma do dispositivo, consulte:</span><span class="sxs-lookup"><span data-stu-id="03d63-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="03d63-106">Configurações de dispositivos Android para configurar e-mail, autenticação e sincronização no Intune</span><span class="sxs-lookup"><span data-stu-id="03d63-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="03d63-107">Adicione as definições de e-mail para dispositivos iOS e iPadOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="03d63-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="03d63-108">Definições de perfil de e-mail no Microsoft Intune para dispositivos que executam o Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="03d63-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="03d63-109">Definições de perfil de e-mail para dispositivos que executam o Windows 10 no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="03d63-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="03d63-110">**Questão comum de sincronização**</span><span class="sxs-lookup"><span data-stu-id="03d63-110">**Common syncing issue**</span></span>

<span data-ttu-id="03d63-111">**Um PERFIL KNOX no Android impede que os Contactos, Calendário e Tarefas dos utilizadores sejam sincronizados com dispositivos do utilizador.**</span><span class="sxs-lookup"><span data-stu-id="03d63-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="03d63-112">O perfil de e-mail KNOX do Android KNOX oferece ao administrador a opção de decidir quais os tipos de conteúdo sincronizados com o dispositivo, definindo cada um para ativar.</span><span class="sxs-lookup"><span data-stu-id="03d63-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="03d63-113">Se a definição de qualquer um dos tipos de conteúdo estiver definida como **Não configurada** (o padrão), esse tipo de conteúdo não é sincronizado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="03d63-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="03d63-114">Um utilizador pode ativar o tipo de conteúdo que pretende diretamente no dispositivo manualmente, mas essa configuração é substituída pela definição de política Intune, e a sincronização para para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="03d63-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

