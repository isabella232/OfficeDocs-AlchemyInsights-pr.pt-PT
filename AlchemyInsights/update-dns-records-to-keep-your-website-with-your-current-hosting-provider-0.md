---
title: Atualizar os registos DNS para manter o seu Web site junto do seu fornecedor de alojamento atual
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423734"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atualizar os registos DNS para manter o seu Web site junto do seu fornecedor de alojamento atual

1. Na página [Domínios](https://portal.office.com/adminportal/home#/Domains), na lista de domínios, selecione o domínio que está a utilizar para o seu site e, em seguida, selecione **Definições de DNS** no painel de gestão. 
    
2. Selecione **+ Novo registo personalizado** e introduza o seguinte: 
    
  - Para **Tipo de DNS**, introduza: **A (Endereço)**
    
  - Em **Nome do anfitrião ou Alias**, escreva o seguinte: **@**
    
  - Em **Endereço IP**, escreva o endereço IP estático onde o seu site está atualmente alojado (por exemplo, 172.16.140.1). 
    
    Tem de ser um endereço IP  *estático*  do site e não um endereço IP  *dinâmico*  . Verifique onde o seu site está alojado para se certificar de que consegue obter um endereço IP estático do seu site público. 
    
3. Selecione **Guardar**. 
    
Além disso, pode criar um registo CNAME para ajudar os clientes a encontrarem o seu site.
  
1. Selecione **+ Novo registo personalizado** e introduza o seguinte: 
    
  - Para **Tipo de DNS**, introduza: **CNAME (Alias)**
    
  - Em **Nome do anfitrião ou Alias**, escreva o seguinte: **www**
    
  - Em **Aponta para o endereço**, escreva o nome de domínio completamente qualificado (FQDN) do site, (por exemplo: contoso.com 
    
2. Selecione **Guardar**. 
    

