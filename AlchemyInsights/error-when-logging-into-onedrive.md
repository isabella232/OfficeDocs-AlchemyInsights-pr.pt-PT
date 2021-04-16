---
title: 0x8004de40 erro ao lançar o OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813663"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="46779-102">0x8004de40 erro ao lançar o OneDrive</span><span class="sxs-lookup"><span data-stu-id="46779-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="46779-103">Se receber um erro **0x8004de40** ao iniciar sessão no OneDrive, reinicie o computador enquanto estiver ligado ao seu trabalho ou domínio escolar.</span><span class="sxs-lookup"><span data-stu-id="46779-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="46779-104">Se receber este erro após o reinício, experimente isto enquanto está ligado ao seu trabalho ou domínio escolar:</span><span class="sxs-lookup"><span data-stu-id="46779-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="46779-105">Clique em Iniciar e **digite cmd** ou pedido de **comando**  na caixa de pesquisa, clique com o botão direito na aplicação de pedido de comando e selecione  **Executar como administrador**.</span><span class="sxs-lookup"><span data-stu-id="46779-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="46779-106">Se for solicitado para uma palavra-passe do administrador ou para uma confirmação, digite a palavra-passe ou clique em **Permitir**.</span><span class="sxs-lookup"><span data-stu-id="46779-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="46779-107">Na janela 'Pedido de Comando', escreva **/saia**  e aguarde que o comando esteja concluído.</span><span class="sxs-lookup"><span data-stu-id="46779-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="46779-108">Em **seguida, escreva dsregcmd /junte-se** e aguarde que o comando esteja completo.</span><span class="sxs-lookup"><span data-stu-id="46779-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="46779-109">Reinicie o seu computador.</span><span class="sxs-lookup"><span data-stu-id="46779-109">Reboot your computer.</span></span>
