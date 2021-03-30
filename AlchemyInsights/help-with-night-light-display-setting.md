---
title: Ajuda com a definição de visualização de luz noturna
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405177"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="34f34-102">Ajuda com a definição de visualização de luz noturna</span><span class="sxs-lookup"><span data-stu-id="34f34-102">Help with the night light display setting</span></span>

<span data-ttu-id="34f34-103">Para saber mais sobre as definições do visor noturno, consulte [definir o seu visor para a noite no Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="34f34-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="34f34-104">Se as opções de luz noturna estiverem acinzentadas nas Definições, verifique o controlador de visualização:</span><span class="sxs-lookup"><span data-stu-id="34f34-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="34f34-105">Clique na caixa de pesquisa na sua barra de tarefas e escreva **o Gestor de Dispositivos** e, em seguida, selecione **o Gestor de Dispositivos** nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="34f34-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="34f34-106">Expandir **os adaptadores do Ecrã**.</span><span class="sxs-lookup"><span data-stu-id="34f34-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="34f34-107">Infelizmente, a função de luz noturna não está disponível se o seu dispositivo utilizar um controlador DisplayLink ou um controlador de exibição básico.</span><span class="sxs-lookup"><span data-stu-id="34f34-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="34f34-108">A função de luz noturna utiliza a tecnologia gráfica recente, pelo que poderá ter de atualizar o controlador de ecrã:</span><span class="sxs-lookup"><span data-stu-id="34f34-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="34f34-109">Verifique se há atualizações indo para **iniciar**  >  a atualização **de definições**  >  **&** verificação da atualização do Windows de segurança  >    >  **para obter atualizações**.</span><span class="sxs-lookup"><span data-stu-id="34f34-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="34f34-110">OU</span><span class="sxs-lookup"><span data-stu-id="34f34-110">OR</span></span>

- <span data-ttu-id="34f34-111">Visite o site de suporte do fabricante de hardware para descarregar manualmente e instalar os controladores de exibição mais recentes.</span><span class="sxs-lookup"><span data-stu-id="34f34-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="34f34-112">Repor a luz noturna no registo</span><span class="sxs-lookup"><span data-stu-id="34f34-112">Reset night light in the registry</span></span>

<span data-ttu-id="34f34-113">Se a atualização do controlador de visualização não funcionar, poderá ter de repor a luz noturna no registo.</span><span class="sxs-lookup"><span data-stu-id="34f34-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="34f34-114">**Atenção:** Este passo de resolução de problemas é recomendado apenas para utilizadores avançados.</span><span class="sxs-lookup"><span data-stu-id="34f34-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="34f34-115">Podem ocorrer problemas graves se modificar o registo incorretamente.</span><span class="sxs-lookup"><span data-stu-id="34f34-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="34f34-116">Para uma proteção adicional, faça uma responsabilidade no registo antes de o modificar para que possa restaurá-lo em caso de problemas.</span><span class="sxs-lookup"><span data-stu-id="34f34-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="34f34-117">Na caixa de pesquisa, **escreva regedit** e, em seguida, selecione **Editor de Registo** nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="34f34-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="34f34-118">Aceda à seguinte chave de registo:</span><span class="sxs-lookup"><span data-stu-id="34f34-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="34f34-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="34f34-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="34f34-120">Exportar e, em seguida, eliminar o seguinte sub-teísta:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="34f34-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="34f34-121">Exporte e, em seguida, elimine o seguinte sub-chave:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="34f34-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="34f34-122">Reinicie o Windows e verifique se as opções de luz noturna estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="34f34-122">Restart Windows and verify if the night light options are available.</span></span>


