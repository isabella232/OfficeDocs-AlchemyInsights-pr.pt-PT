---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734317"
---
# <a name="verify-your-domain"></a><span data-ttu-id="cfa37-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="cfa37-102">Verify your domain</span></span>

 <span data-ttu-id="cfa37-103">**O registo provavelmente não se atualizou na Internet.**</span><span class="sxs-lookup"><span data-stu-id="cfa37-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="cfa37-104">Normalmente só leva alguns minutos para podermos ver o novo disco, mas ocasionalmente pode levar o tempo que for algumas horas.</span><span class="sxs-lookup"><span data-stu-id="cfa37-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="cfa37-105">Se já esperou tanto tempo, verifique duas vezes que copiou e colou o valor exato no registo de verificação do TXT no seu anfitrião DNS.</span><span class="sxs-lookup"><span data-stu-id="cfa37-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="cfa37-106">Um problema comum é não incluir a parte "MS=" do registo.</span><span class="sxs-lookup"><span data-stu-id="cfa37-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="cfa37-107">Também precisamos disso!</span><span class="sxs-lookup"><span data-stu-id="cfa37-107">We need that too!</span></span>

- <span data-ttu-id="cfa37-108">Em alguns anfitriões de DNS, tem de efetuar um passo adicional para guardar o ficheiro de zona (onde o registo DNS é armazenado) para que seja atualizado na Internet.</span><span class="sxs-lookup"><span data-stu-id="cfa37-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="cfa37-109">Certifique-se de que guardou as suas alterações para que a Microsoft possa ver e verificar o registo.</span><span class="sxs-lookup"><span data-stu-id="cfa37-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
