---
title: A classificação automática não está a funcionar conforme esperado com o cliente do AIP
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979720"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>A classificação automática não está a funcionar conforme esperado com o cliente do AIP

A classificação automática não está a funcionar conforme esperado. Utilize as seguintes diretrizes recomendadas:

1. Se estiver a ter problemas com a etiquetagem automática, consulte [Como configurar condições para a classificação automática e recomendada do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [O que os tipos de informação confidencial procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Verifique se está a utilizar políticas com âmbito que não estão configuradas corretamente: [Como configurar a política do Azure Information Protection para utilizadores específicos ao utilizar políticas com âmbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Se a etiquetagem automática não estiver a funcionar no Outlook ao anexar um documento com etiqueta, verifique se `DRMEncryptProperty` não está definido conforme descrito aqui: [definições de registo da IRM para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Se utilizou os [tipos de informação incorporados](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) da sua política do Azure Information Protection, verifique se os seus conteúdos correspondem ao formato esperado.
5. Verifique se a etiqueta está corretamente configurada como **Automática** ou **Recomendada**. (A etiquetagem **Automática** está disponível para todas as aplicações do Microsoft 365, ao passo que a **Recomendada** está disponível para todas as aplicações do Microsoft 365 exceto Outlook.)
6. Não pode utilizar a classificação automática para documentos e e-mails que foram anteriormente etiquetados manual ou automaticamente com uma classificação mais alta.  Para obter mais informações, consulte: [Como são aplicadas as etiquetas automáticas ou recomendadas](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Se ainda estiver a deparar-se com problemas, recolha os registos de cliente do Azure Information Protection e anexe os registos exportados ao seu pedido de suporte. Para exportar registos do Azure Information Protection:
    - Abra um documento do Office ou crie um novo e-mail no Outlook.
    - Clique em **Proteger/Confidencialidade** > **Ajuda e comentários**.
    - Clique em **Exportar Registos**.
    - Guarde os registos numa localização à sua escolha e anexe-os ao seu pedido de serviço.

Para obter mais informações, consulte:

- [Como configurar condições para a classificação automática e recomendada do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Manuais de instruções para cenários comuns que envolvem o Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Rever a documentação do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Rever as subscrições e funcionalidades do Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Requisitos do Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tutorial de início rápido para o Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Transferir cliente do Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
