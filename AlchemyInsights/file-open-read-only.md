---
title: Arquivo aberto apenas leitura
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745618"
---
# <a name="file-open-read-only"></a><span data-ttu-id="67058-102">Arquivo aberto apenas leitura</span><span class="sxs-lookup"><span data-stu-id="67058-102">File open read-only</span></span>

<span data-ttu-id="67058-103">Pode descobrir que quando estiver a abrir ficheiros, eles abrem-se apenas para ler.</span><span class="sxs-lookup"><span data-stu-id="67058-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="67058-104">Em alguns casos, isto é para uma segurança acrescida, como quando está a abrir ficheiros a partir da internet, e outras vezes, pode ser devido a uma configuração que pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="67058-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="67058-105">Aqui estão alguns cenários em que um ficheiro abre apenas a leitura e alguns passos que pode tomar para mudar isso.</span><span class="sxs-lookup"><span data-stu-id="67058-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="67058-106">**O meu antivírus está a fazê-los abrir apenas a leitura.**</span><span class="sxs-lookup"><span data-stu-id="67058-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="67058-107">Alguns programas antivírus podem protegê-lo de ficheiros potencialmente inseguros abrindo-os apenas de leitura.</span><span class="sxs-lookup"><span data-stu-id="67058-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="67058-108">Poderá ser necessário consultar o seu fornecedor antivírus para aprender a ajustar estas definições.</span><span class="sxs-lookup"><span data-stu-id="67058-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="67058-109">O BitDefender, por exemplo, tem conteúdo na adição de exclusões de aplicações aqui: [Como adicionar exclusões de aplicações ou processos no Centro de Controlo de Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="67058-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="67058-110">**As propriedades do ficheiro estão definidas apenas para ler?**</span><span class="sxs-lookup"><span data-stu-id="67058-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="67058-111">Pode verificar as propriedades do ficheiro clicando corretamente no ficheiro e escolhendo propriedades.</span><span class="sxs-lookup"><span data-stu-id="67058-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="67058-112">Se o atributo Read-only for verificado, pode desacompi-lo e clicar em OK.</span><span class="sxs-lookup"><span data-stu-id="67058-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="67058-113">**O conteúdo está na vista protegida**</span><span class="sxs-lookup"><span data-stu-id="67058-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="67058-114">Ficheiros da Internet e de outros locais potencialmente inseguros podem conter vírus, worms ou outros tipos de malware que podem prejudicar o seu computador.</span><span class="sxs-lookup"><span data-stu-id="67058-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="67058-115">Este também é geralmente o caso com anexos de e-mail ou ficheiros que você descarregou.</span><span class="sxs-lookup"><span data-stu-id="67058-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="67058-116">Para ajudar a proteger o seu computador, os ficheiros destes locais potencialmente inseguros são abertos em Protected View.</span><span class="sxs-lookup"><span data-stu-id="67058-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="67058-117">Ao utilizar a ProtectEd View, pode ler um ficheiro e ver o seu conteúdo, reduzindo os riscos.</span><span class="sxs-lookup"><span data-stu-id="67058-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="67058-118">Para obter mais informações sobre a vista protegida e como alterar as definições, consulte este artigo: [O que é a Vista Protegida?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="67058-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="67058-119">**O OneDrive está cheio?**</span><span class="sxs-lookup"><span data-stu-id="67058-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="67058-120">Se o ficheiro estiver armazenado no OneDrive e o seu espaço de armazenamento OneDrive estiver cheio, não poderá guardar o documento até estar sob o seu espaço atribuído.</span><span class="sxs-lookup"><span data-stu-id="67058-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="67058-121">Pode verificar o seu espaço gratuito no OneDrive clicando no ícone OneDrive no centro de notificação e escolhendo o armazenamento de Manage, ou pode [https://onedrive.live.com](https://onedrive.live.com) ir, iniciar sôm e observar a quantidade de espaço usado na parte inferior esquerda do ecrã.</span><span class="sxs-lookup"><span data-stu-id="67058-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="67058-122">**O Escritório está ativado?**</span><span class="sxs-lookup"><span data-stu-id="67058-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="67058-123">Se o Office não estiver ativado ou se a sua subscrição tiver expirado, poderá estar no modo de funcionalidade reduzida apenas de leitura.</span><span class="sxs-lookup"><span data-stu-id="67058-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="67058-124">Para obter informações sobre como ativar o Escritório, consulte: [Erros de produto não licenciados e erros de ativação no Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="67058-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="67058-125">**Se tudo o resto falhar...**</span><span class="sxs-lookup"><span data-stu-id="67058-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="67058-126">Tente reiniciar o computador</span><span class="sxs-lookup"><span data-stu-id="67058-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="67058-127">Instalar atualizações do Office</span><span class="sxs-lookup"><span data-stu-id="67058-127">Install Office updates</span></span>
    
- <span data-ttu-id="67058-128">Realizar uma reparação online do Office</span><span class="sxs-lookup"><span data-stu-id="67058-128">Perform an Online repair of Office</span></span>
    

