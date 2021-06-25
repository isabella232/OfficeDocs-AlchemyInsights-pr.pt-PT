---
title: Reencaminhamento de e-mail através do Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117994"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Configurar uma aplicação ou dispositivo multifunções para enviar e-mails

Para obter mais informações sobre os passos e opções disponíveis, consulte [Como configurar uma aplicação ou dispositivo multifunções para enviar e-mails com o Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Se tiver um dispositivo ou aplicação que deixou de funcionar recentemente, os problemas mais comuns são:

- **Erros relacionados com a autenticação ao utilizar a submissão de cliente SMTP Auth** Recentemente, fizemos algumas alterações relacionadas com o funcionamento da Autenticação SMTP. Para obter mais informações sobre como resolver problemas, consulte a secção de autenticação sem sucesso da secção Corrigir problemas com impressoras, [scanners](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)e aplicações LOB que enviam e-mails através de Microsoft 365 ou Office 365.
- **Aceitamos apenas a versão TLS 1.2 ao criar uma ligação segura ao Office 365** Se estiver a utilizar Uma Ligação Segura (TLS), certifique-se de que o seu dispositivo de aplicação suporta TLS 1.2. Para obter mais informações, [consulte Preparar para o TLS 1.2 no Office 365 e Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Para outros problemas e soluções, consulte Corrigir problemas com impressoras, [scanners](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)e aplicações LOB que enviam e-mails através Microsoft 365 ou Office 365.

Para ver os dispositivos afetados, aceda ao [relatório dos Clientes de Autenticação de SMTP](https://protection.office.com/mailflow/dashboard)

**Nota:** Exchange Online não acomoda cenários de correio em massa. Para enviar e-mails comerciais em massa (por exemplo, newsletters de clientes), deve utilizar fornecedores de terceiros especializados nestes serviços.
