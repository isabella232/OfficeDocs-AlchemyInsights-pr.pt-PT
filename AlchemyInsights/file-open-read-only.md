---
title: Arquivo aberto somente leitura
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822245"
---
# <a name="file-open-read-only"></a><span data-ttu-id="cce21-102">Arquivo aberto somente leitura</span><span class="sxs-lookup"><span data-stu-id="cce21-102">File open read-only</span></span>

<span data-ttu-id="cce21-103">Você pode achar que quando você está abrindo arquivos, eles abrem como somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce21-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="cce21-104">Em alguns casos, isso é para segurança adicional, como quando você está abrindo arquivos da Internet e outras vezes, pode ser devido a uma configuração que pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="cce21-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="cce21-105">Aqui estão alguns cenários em que um arquivo abre somente leitura e algumas etapas que você pode tomar para alterá-lo.</span><span class="sxs-lookup"><span data-stu-id="cce21-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="cce21-106">**Meu antivírus está fazendo com que eles abram somente leitura**</span><span class="sxs-lookup"><span data-stu-id="cce21-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="cce21-107">Alguns programas antivírus podem protegê-lo de arquivos potencialmente não seguros, abrindo-os somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce21-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="cce21-108">Talvez seja necessário verificar com seu provedor de antivírus para saber como ajustar essas configurações.</span><span class="sxs-lookup"><span data-stu-id="cce21-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="cce21-109">O BitDefender, por exemplo, tem conteúdo para adicionar exclusões de aplicações aqui: [como adicionar exclusões de aplicações ou processos no centro de controlo BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="cce21-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="cce21-110">**As propriedades do arquivo são definidas como somente leitura?**</span><span class="sxs-lookup"><span data-stu-id="cce21-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="cce21-111">Você pode verificar as propriedades do arquivo clicando com o botão direito do mouse no arquivo e escolhendo Propriedades.</span><span class="sxs-lookup"><span data-stu-id="cce21-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="cce21-112">Se o atributo somente leitura estiver marcado, você poderá desmarcá-lo e clicar em OK.</span><span class="sxs-lookup"><span data-stu-id="cce21-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="cce21-113">**O conteúdo está em modo de exibição protegido**</span><span class="sxs-lookup"><span data-stu-id="cce21-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="cce21-114">Os arquivos da Internet e de outros locais potencialmente inseguros podem conter vírus, worms ou outros tipos de malware que podem prejudicar seu computador.</span><span class="sxs-lookup"><span data-stu-id="cce21-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="cce21-115">Isso também é comumente o caso com anexos de e-mail ou arquivos que você baixou.</span><span class="sxs-lookup"><span data-stu-id="cce21-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="cce21-116">Para ajudar a proteger seu computador, os arquivos desses locais potencialmente inseguros são abertos no modo de exibição protegido.</span><span class="sxs-lookup"><span data-stu-id="cce21-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="cce21-117">Usando o modo de exibição protegido, você pode ler um arquivo e ver seu conteúdo, reduzindo os riscos.</span><span class="sxs-lookup"><span data-stu-id="cce21-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="cce21-118">Para obter mais informações sobre o modo de exibição protegido e como alterar as configurações, consulte este artigo: [o que é o modo de exibição protegido?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="cce21-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="cce21-119">**O OneDrive está cheio?**</span><span class="sxs-lookup"><span data-stu-id="cce21-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="cce21-120">Se o arquivo estiver armazenado no OneDrive e seu espaço de armazenamento do OneDrive estiver cheio, você não poderá salvar o documento até que esteja seu espaço alocado.</span><span class="sxs-lookup"><span data-stu-id="cce21-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="cce21-121">Você pode verificar seu espaço livre no OneDrive clicando no ícone do OneDrive na central de notificações e escolhendo gerenciar armazenamento, ou você pode ir para [http://onedrive.live.com](http://onedrive.live.com), entrar e observe a quantidade de espaço usado no canto inferior esquerdo da tela.</span><span class="sxs-lookup"><span data-stu-id="cce21-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="cce21-122">**O Office está activado?**</span><span class="sxs-lookup"><span data-stu-id="cce21-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="cce21-123">Se o Office não estiver ativado ou se sua assinatura expirar, você poderá estar no modo de funcionalidade reduzida somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce21-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="cce21-124">Para obter informações sobre como ativar o Office, consulte: [produtos não licenciados e erros de ativação no Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="cce21-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="cce21-125">**Se tudo mais falhar...**</span><span class="sxs-lookup"><span data-stu-id="cce21-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="cce21-126">Tente reiniciar o computador</span><span class="sxs-lookup"><span data-stu-id="cce21-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="cce21-127">Instalar atualizações do Office</span><span class="sxs-lookup"><span data-stu-id="cce21-127">Install Office updates</span></span>
    
- <span data-ttu-id="cce21-128">Realize uma reparação online do Office</span><span class="sxs-lookup"><span data-stu-id="cce21-128">Perform an Online repair of Office</span></span>
    

