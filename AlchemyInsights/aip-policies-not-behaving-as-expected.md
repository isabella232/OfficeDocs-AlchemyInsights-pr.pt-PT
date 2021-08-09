---
title: 'AIP: As políticas não se comportam conforme esperado'
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
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934304"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: As políticas não se comportam conforme esperado

Azure Information Protection: As políticas não se comportam conforme esperado, consulte as seguintes diretrizes recomendadas para diversos problemas de política:

1. Se estiver a ter problemas com marcações visuais, consulte Quando são [aplicadas marcações visuais.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Se estiver a ter problemas com a etiquetagem automática, consulte Como configurar condições para a classificação automática e recomendada para o [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e O que os tipos de informação confidenciais [procuram.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Se estiver a ter problemas com a proteção Nativa/Pfile, reveja a [configuração da API de Ficheiros.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Verifique se está a utilizar políticas com âmbito que não estão configuradas corretamente: [Como configurar a política do Azure Information Protection para utilizadores específicos ao utilizar políticas com âmbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Se a etiqueta automática não estiver a funcionar com o Outlook ao anexar um documento com etiquetas, verifique se DRMEncryptProperty não está definido como descrito aqui: DEFINIÇÕES de [registo IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)para segurança .

Se continuar a ter problemas, recolha os registos do cliente do Azure Information Protection e anexe os registos exportados a este pedido.

1. Abra um documento do Office ou crie um novo e-mail no Outlook.
2. Clique em **Proteger/Confidencialidade** > **Ajuda e comentários**.
3. Clique em **Exportar Registos**.
4. Guarde os registos na sua escolha de localização e anexe-os a este pedido de serviço.

Recursos adicionais:

- [Como configurar uma etiqueta para marcações visuais para o Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Rever a documentação do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Utilizar etiquetas de sensibilidade em Microsoft 365 aplicações](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

