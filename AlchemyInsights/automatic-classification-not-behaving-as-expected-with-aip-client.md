---
title: Classificação automática não se comporta como esperado com o cliente AIP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508387"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Classificação automática não se comporta como esperado com o cliente AIP

Classificação automática não se comporta como esperado, utilize as seguintes orientações recomendadas:

1. Se tiver problemas com a rotulagem automática, consulte [como configurar condições para classificação automática e recomendada para a Proteção de Informação Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [quais os tipos de informação sensíveis procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Verifique se está a utilizar políticas de âmbito que não estejam configuradas corretamente: [Como configurar a política de proteção de informação Azure para utilizadores específicos utilizando políticas de âmbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Se a rotulagem automática não estiver a funcionar para o Outlook ao anexar um documento rotulado, verifique se `DRMEncryptProperty` não está definido como descrito aqui: [Definições de registo de IRM para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Se utilizar os [tipos de informação incorporada](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) para a sua política de Proteção de Informações Azure, verifique se o seu conteúdo corresponde ao formato esperado.
5. Verifique se a etiqueta está adequadamente configurada para **Automática** ou **Recomendada**. (A rotulagem**automática** está disponível para todas as aplicações do Office, enquanto **recomendada** está disponível para todas as aplicações do Office, exceto para o Outlook.)
6. Não é possível utilizar a classificação automática para documentos e e-mails previamente rotulados manualmente ou previamente rotulados automaticamente com uma classificação superior.  Para obter mais informações, consulte: [Como são aplicadas etiquetas automáticas ou recomendadas](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Se ainda estiver com problemas, por favor, recolha os registos do cliente da Azure Information Protection e anexe os registos exportados ao seu bilhete de suporte. Para exportar registos de proteção de informação Azure:
    - Abra um documento do Office ou crie um novo e-mail no Outlook.
    - Clique **em Proteger/Sensibilidade**  >  **Ajuda e feedback**.
    - Clique em **Registos de Exportação**.
    - Guarde os registos à sua escolha de localização e anexe-os ao seu pedido de serviço.

Para obter informações adicionais, consulte:

- [Como configurar condições para classificação automática e recomendada para proteção de informação do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Guias para cenários comuns que utilizam a Proteção de Informação do Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Rever documentação de proteção de informação do Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Rever subscrições e funcionalidades da Proteção de Informação Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Requisitos para a proteção da informação do Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tutorial de início rápido para proteção de informação do Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Baixar cliente da Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
