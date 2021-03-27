---
title: Conceitos avançados de autenticação aplicáveis ao Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398596"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="3635b-102">Conceitos avançados de autenticação aplicáveis ao Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3635b-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="3635b-103">Seguem-se os conceitos avançados de autenticação aplicáveis ao Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="3635b-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="3635b-104">**Autenticação Proativa**</span><span class="sxs-lookup"><span data-stu-id="3635b-104">**Proactive Authentication**</span></span>

<span data-ttu-id="3635b-105">Quando ativar a política [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) o Microsoft Edge tentará autenticar proactivamente os utilizadores inscritos através dos serviços da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3635b-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="3635b-106">Em intervalos regulares, utilizará um serviço online para verificar se há um manifesto atualizado que contenha a configuração que rege a Autenticação Proactiva.</span><span class="sxs-lookup"><span data-stu-id="3635b-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="3635b-107">Benefícios: A autenticação proativa permite a autenticação em serviços-chave, como a Página do Separador Do Office New.</span><span class="sxs-lookup"><span data-stu-id="3635b-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="3635b-108">Além disso, se bing é usado como motor de pesquisa, a Autenticação Proativa melhora o desempenho da barra de endereços e ajuda a gerar resultados de pesquisa personalizados às necessidades do seu negócio.</span><span class="sxs-lookup"><span data-stu-id="3635b-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="3635b-109">**Windows Hello CredUI para autenticação NTLM**</span><span class="sxs-lookup"><span data-stu-id="3635b-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="3635b-110">Se um único sign-on (SSO) não estiver disponível quando um website tentar assinar no utilizador através do mecanismo NTLM ou Negotiate, esta funcionalidade permitirá ao utilizador partilhar as credenciais de OS com o website e satisfazer o desafio de autenticação utilizando o UI do Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="3635b-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="3635b-111">Este fluxo de entrada de sing-on aparecerá apenas no Windows 10 e apenas para utilizadores que não obtenham SSO durante um NTLM ou um desafio Negotiate.</span><span class="sxs-lookup"><span data-stu-id="3635b-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="3635b-112">**Utilize senhas guardadas para iniciar sôm automaticamente**</span><span class="sxs-lookup"><span data-stu-id="3635b-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="3635b-113">Os utilizadores que guardam palavras-passe no Microsoft Edge podem permitir o acesso automático aos websites onde guardaram credenciais.</span><span class="sxs-lookup"><span data-stu-id="3635b-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="3635b-114">Os utilizadores podem ligar ou desligar esta funcionalidade em edge://settings/passwords, podendo configugá-la nas políticas do [gestor de passwords.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="3635b-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
