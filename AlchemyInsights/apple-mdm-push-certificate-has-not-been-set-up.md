---
title: Apple MDM Push Certificate ainda não foi criado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440014"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push Certificate ainda não foi criado

Um Certificado de Pressão MD da Apple (também conhecido como certificado apple push notification service (APNS) não foi configurado para a sua subscrição. Sem um Certificado de Pressão Apple MDM configurado, não é possível inscrever e gerir dispositivos iOS e Mac OS. Depois de adicionar o certificado ao Intune, os utilizadores podem instalar a aplicação Portal da Empresa para inscrever os seus dispositivos iOS.

1. **Selecione "Concordo".** para dar permissão à Microsoft para enviar dados para a Apple.

2. Selecione **Descarregue o seu** pedido de assinatura de certificado Intune necessário para criar um certificado de pressão Apple MDM. O ficheiro é utilizado para solicitar um certificado de relação fiduciuada do Portal dos Certificados Apple Push.

3. Selecione **Crie o seu certificado de push MDM** para ir ao Portal dos Certificados apple push. Inscreva-se com a sua empresa Apple ID e, em seguida, **selecione Criar um Certificado**. Selecione **Choose File,** navegue no ficheiro de pedido de assinatura de certificado e, em seguida, escolha **Upload**. Na página Confirmação, escolha **Descarregar** para descarregar o ficheiro certificado (.pem) e guardar o ficheiro localmente.
 
**Nota:** O certificado está associado ao Apple ID utilizado para criá-lo. Como uma boa prática, use uma empresa Apple ID para tarefas de gestão, e certifique-se de que a caixa de correio é monitorizada por mais de uma pessoa ou usando uma lista de distribuição. Nunca utilize um Apple ID pessoal. Use o mesmo Apple ID para renovar o Apple Push Certificate a cada 12 meses.
 
4. Introduza o Apple ID usado para criar o seu certificado de push Apple MDM. Grave este ID como um lembrete para quando precisar de renovar o certificado.

5. Vá ao arquivo de certificado (.pem), escolha **Open**e, em seguida, escolha **Upload**. Com o certificado push, o Intune pode inscrever-se e gerir dispositivos Apple.