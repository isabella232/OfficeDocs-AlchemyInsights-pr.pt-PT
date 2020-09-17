---
title: Atualizar os registos DNS para manter o seu Web site junto do seu fornecedor de alojamento atual
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815796"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atualizar os registos DNS para manter o seu Web site junto do seu fornecedor de alojamento atual

1. No centro de administração microsoft 365, vá à página De Domínios de **Configuração**  >  [Domains](https://admin.microsoft.com/Adminportal#/Domains) e na lista de domínios, selecione o domínio que está a utilizar para o seu website.

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
