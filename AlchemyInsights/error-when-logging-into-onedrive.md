---
title: Erro 0x8004de40 ao lançar o OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823114"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="689e2-102">Erro 0x8004de40 ao lançar o OneDrive</span><span class="sxs-lookup"><span data-stu-id="689e2-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="689e2-103">Se receber um erro **0x8004de40** ao iniciar sessão no OneDrive, reinicie o computador enquanto estiver ligado ao seu trabalho ou domínio escolar.</span><span class="sxs-lookup"><span data-stu-id="689e2-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="689e2-104">Se receber este erro após o reinício, experimente isto enquanto está ligado ao seu trabalho ou domínio escolar:</span><span class="sxs-lookup"><span data-stu-id="689e2-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="689e2-105">Clique em Iniciar e **digite cmd** ou pedido de **comando**  na caixa de pesquisa, clique com o botão direito na aplicação de pedido de comando e selecione  **Executar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="689e2-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="689e2-106">Se for solicitado para uma palavra-passe do administrador ou para uma confirmação, digite a palavra-passe ou clique em **Permitir** .</span><span class="sxs-lookup"><span data-stu-id="689e2-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="689e2-107">Na janela 'Pedido de Comando', escreva **/saia**  e aguarde que o comando esteja concluído.</span><span class="sxs-lookup"><span data-stu-id="689e2-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="689e2-108">Em **seguida, escreva dsregcmd /junte-se** e aguarde que o comando esteja completo.</span><span class="sxs-lookup"><span data-stu-id="689e2-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="689e2-109">Reinicie o seu computador.</span><span class="sxs-lookup"><span data-stu-id="689e2-109">Reboot your computer.</span></span>
