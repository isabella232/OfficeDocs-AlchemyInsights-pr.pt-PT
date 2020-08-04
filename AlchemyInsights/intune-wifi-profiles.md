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
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="e1b5c-102">Perfis Wi-Fi intune</span><span class="sxs-lookup"><span data-stu-id="e1b5c-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="e1b5c-103">A implementação bem sucedida da conectividade Wi-Fi para clientes MDM depende de um perfil corretamente implantado que reflita os requisitos da infraestrutura Wi-Fi corporativa.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="e1b5c-104">Para rever as definições apropriadas para as plataformas de clientes que está a investigar, consulte:</span><span class="sxs-lookup"><span data-stu-id="e1b5c-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="e1b5c-105">Adicione definições de Wi-Fi para dispositivos que executam o Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e1b5c-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="e1b5c-106">Adicione definições de Wi-Fi para dispositivos dedicados e totalmente geridos do Android Enterprise no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e1b5c-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="e1b5c-107">Adicione definições wi-fi para dispositivos iOS e iPadOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e1b5c-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="e1b5c-108">Adicione definições de Wi-Fi para windows 10 e dispositivos posteriores no Intune</span><span class="sxs-lookup"><span data-stu-id="e1b5c-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="e1b5c-109">Importar definições de Wi-Fi para dispositivos Windows em Intune</span><span class="sxs-lookup"><span data-stu-id="e1b5c-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="e1b5c-110">**Questões Comuns**</span><span class="sxs-lookup"><span data-stu-id="e1b5c-110">**Common Issues**</span></span>

<span data-ttu-id="e1b5c-111">**Estou a implantar um perfil Wi-Fi que depende de um certificado implantado especificado no perfil Wi-Fi. No entanto, os perfis de configuração mostram um estado de erro.**</span><span class="sxs-lookup"><span data-stu-id="e1b5c-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="e1b5c-112">Verifique se o seu dispositivo recebeu o certificado.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="e1b5c-113">No Intune, vá a **todos os dispositivos** e selecione o dispositivo > **configuração do dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="e1b5c-114">Verifique se todos os perfis esperados estão listados e em estado de sucesso.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="e1b5c-115">Para um perfil Android, se tiver certificados intermédios na sua cadeia de certificados, certifique-se de que são implantados em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="e1b5c-116">Para verificar o estado do certificado, aceda aos perfis **de configuração do Dispositivo**Android intermediate  >  **Profiles**  >  **CA**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="e1b5c-117">Se continuar a ver erros, reveja os procedimentos e as secções de resolução de problemas.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="e1b5c-118">Para obter mais informações, consulte [a Visão Geral para resolver os perfis de certificados SCEP com o Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e1b5c-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="e1b5c-119">**Desloquei um perfil Wi-Fi para um dispositivo. A Intune está a mostrar que foi bem sucedida, mas o dispositivo não está a ligar-se ao Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="e1b5c-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="e1b5c-120">Um estado de sucesso significa que a Intune implementou o perfil com sucesso como configurado.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="e1b5c-121">No entanto, estas configurações podem não corresponder aos seus requisitos de rede e/ou autenticação.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="e1b5c-122">Para obter mais detalhes sobre a tentativa de ligação, reveja os registos na infraestrutura e no serviço de autenticação (no controlador de ponto de acesso Wi-Fi e no servidor NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="e1b5c-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="e1b5c-123">Você pode ter que trabalhar com a sua equipa de infraestrutura de rede, ou o fornecedor de Wi-Fi de terceiros, para recolher e rever registos.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>