---
title: Criação de políticas de etiquetas AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569508"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="b886b-102">Criação de políticas de etiquetas AIP</span><span class="sxs-lookup"><span data-stu-id="b886b-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="b886b-103">As etiquetas Azure Information Protection (AIP) podem ser utilizadas com toda a gama de dados que uma organização normalmente cria e armazena, desde a classificação mais baixa dos dados pessoais, até à classificação mais elevada de dados altamente confidenciais.</span><span class="sxs-lookup"><span data-stu-id="b886b-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="b886b-104">As Políticas de Proteção da Informação Azure aplicam-se ao cliente clássico da Azure Information Protection (AIP) e não ao [cliente de rotulagem unificada da AIP.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)</span><span class="sxs-lookup"><span data-stu-id="b886b-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="b886b-105">Pode configurar vários elementos numa política AIP, incluindo opções como:</span><span class="sxs-lookup"><span data-stu-id="b886b-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="b886b-106">Opção para a qual o rótulo permitirá aos administradores ou utilizador classificar e proteger documentos e e-mails (opcional)</span><span class="sxs-lookup"><span data-stu-id="b886b-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="b886b-107">Opção de impor classificação quando os utilizadores guardam documentos e enviam e-mail</span><span class="sxs-lookup"><span data-stu-id="b886b-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="b886b-108">Opção de rotular automaticamente uma mensagem de e-mail, com base nos seus anexos.</span><span class="sxs-lookup"><span data-stu-id="b886b-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="b886b-109">Opção de controlar se a barra de proteção de informação é apresentada em aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="b886b-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="b886b-110">Para opções adicionais e informações sobre as políticas de proteção da informação do Azure, consulte: [Visão geral da política de proteção de informação Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="b886b-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="b886b-111">Para outros recursos úteis no que diz respeito às políticas AIP, consulte:</span><span class="sxs-lookup"><span data-stu-id="b886b-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="b886b-112">Tutorial: Configurar as definições da política de proteção da informação do Azure e criar um novo rótulo</span><span class="sxs-lookup"><span data-stu-id="b886b-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b886b-113">Configurar a política de proteção da informação do Azure</span><span class="sxs-lookup"><span data-stu-id="b886b-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="b886b-114">Criar e configurar rótulos de sensibilidade e suas políticas</span><span class="sxs-lookup"><span data-stu-id="b886b-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="b886b-115">Guias para cenários comuns que utilizam a Proteção de Informação do Azure</span><span class="sxs-lookup"><span data-stu-id="b886b-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="b886b-116">Rever documentação de proteção de informação do Azure</span><span class="sxs-lookup"><span data-stu-id="b886b-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="b886b-117">Requisitos para a proteção da informação do Azure</span><span class="sxs-lookup"><span data-stu-id="b886b-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="b886b-118">Tutorial de início rápido para proteção de informação do Azure</span><span class="sxs-lookup"><span data-stu-id="b886b-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b886b-119">Baixar cliente da Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b886b-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)