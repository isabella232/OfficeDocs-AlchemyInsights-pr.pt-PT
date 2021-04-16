---
title: Gerir a lista de endereços global da organização e o livro de endereços offline
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
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794843"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="17640-102">Gerir a lista de endereços global (GAL) da organização e o livro de endereços offline (OAB)</span><span class="sxs-lookup"><span data-stu-id="17640-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="17640-103">Uma lista de endereços global (GAL) é uma lista de objetos com capacidade de correio (qualquer tipo de destinatário que possa receber e-mails) na organização.</span><span class="sxs-lookup"><span data-stu-id="17640-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="17640-104">Uma GAL é criada automaticamente em todas as organizações.</span><span class="sxs-lookup"><span data-stu-id="17640-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="17640-105">Pode criar GALs adicionais para separar os utilizadores por organização ou localização, mas cada utilizador só pode ver e usar uma GAL de cada vez.</span><span class="sxs-lookup"><span data-stu-id="17640-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="17640-106">Alguns clientes de e-mail, como o Outlook para Windows, transferem a GAL para uso offline.</span><span class="sxs-lookup"><span data-stu-id="17640-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="17640-107">Esta funcionalidade é conhecida como livro de endereços offline (OAB).</span><span class="sxs-lookup"><span data-stu-id="17640-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="17640-108">No Exchange online, o OAB é atualizado a cada 8 horas. Após a atualização, o cliente tem de o transferir para atualizar a cópia local do OAB.</span><span class="sxs-lookup"><span data-stu-id="17640-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="17640-109">Qualquer alteração de destinatário tem de ser primeiro visível na GAL para ser, então, refletida no OAB.</span><span class="sxs-lookup"><span data-stu-id="17640-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="17640-110">Aqui estão alguns procedimentos da GAL e do OAB comumente usados:</span><span class="sxs-lookup"><span data-stu-id="17640-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="17640-111">Por várias razões, pode pretender que alguns objetos sejam escondidos da GAL.</span><span class="sxs-lookup"><span data-stu-id="17640-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="17640-112">Consulte [Ocultar destinatários de listas de endereços](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="17640-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="17640-113">Se precisar de fornecer vistas personalizadas da GAL da organização a grupos específicos de utilizadores, consulte[Políticas do livro de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="17640-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="17640-114">[Criar uma lista de endereços global no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) e, para saber como trabalhar com as permissões da GAL, consulte [Listas de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="17640-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="17640-115">Tenha em atenção que se criar uma nova GAL também pode querer criar um novo OAB.</span><span class="sxs-lookup"><span data-stu-id="17640-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="17640-116">Consulte [Procedimentos do livro de endereços](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="17640-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
