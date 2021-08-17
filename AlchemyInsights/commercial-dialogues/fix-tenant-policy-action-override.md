---
title: Corrigir política de inquilino (override de ação)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896086"
---
# <a name="fix-tenant-policy-action-override"></a>Corrigir política de inquilino (override de ação)

Uma das suas políticas antisspam afetou esta mensagem. Para rever as políticas, faça o seguinte:

1. No portal Microsoft 365 Defender, em , vá para E-mail & políticas de <https://security.microsoft.com/>  \> **colaboração & Regras** \>  \> **contra ameaças Antisspam,** na **secção** Políticas.

   Para ir diretamente para a **página Políticas antisspam,** utilize <https://security.microsoft.com/antispam> .

2. Na página Políticas **antisspam,** selecione a política ao clicar no nome da  política **(** Tipo é Política **antisspam** personalizada ou Nome é Política de receção Antisspam **(Predefinição).**
3. Na panfleto de detalhes que é exibida, **selecione Editar ações** na **secção Ações.**
4. Na secção Ações **de** mensagens, reveja os vereditos de **Spam, Spam** de alta confiança, Phishing e  **Phishing** de Confiança Alta para ver se algum dos seguintes valores está selecionado: 
   - **Adicionar cabeçalho X**
   - **Pré-abrir o assunto da mensagem com texto**
   - **Redirecionar a mensagem para o endereço de e-mail**
   - **Eliminar mensagem**
   - **Sem ação**

   É possível que as definições **Padrão aplicadas a** todos os Proteção do Exchange Online clientes afetaram a mensagem.

Para obter mais informações, [consulte Configurar políticas antisspam na EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
