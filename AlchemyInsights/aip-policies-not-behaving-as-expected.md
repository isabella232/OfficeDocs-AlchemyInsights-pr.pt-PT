---
title: 'AIP: Políticas que não se comportam como esperado'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663200"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Políticas que não se comportam como esperado

Azure Information Protection: Políticas que não se comportam como esperado, consulte as seguintes orientações recomendadas para várias questões políticas:

1. Se tiver problemas com as marcas visuais, reveja [quando as marcas visuais forem aplicadas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Se tiver problemas com a rotulagem automática, [reveja como configurar as condições para a classificação automática e recomendada para a Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [quais os tipos de informação sensíveis procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Se tiver problemas com a proteção Native/Pfile, por favor reveja [a configuração da API do ficheiro](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Verifique se está a utilizar políticas de âmbito que não estejam configuradas corretamente: [Como configurar a política de proteção de informação Azure para utilizadores específicos utilizando políticas de âmbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Se a rotulagem automática não estiver a funcionar para o Outlook ao anexar um documento rotulado, verifique se a DRMEncryptProperty não está definida como descrito aqui: [Definições de registo irm para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Se ainda estiver com problemas, por favor, recolha os registos de clientes da Azure Information Protection e anexe os registos exportados a este bilhete.

1. Abra um documento do Office ou crie um novo e-mail no Outlook.
2. Clique **em Proteger/Sensibilidade**  >  **Ajuda e feedback**.
3. Clique em **Registos de Exportação**.
4. Guarde os registos à sua escolha de localização e anexe-os a este pedido de serviço.

Recursos adicionais:

- [Como configurar um rótulo para marcações visuais para proteção de informação Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Rever documentação de proteção de informação do Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Utilize etiquetas de sensibilidade em aplicações microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

