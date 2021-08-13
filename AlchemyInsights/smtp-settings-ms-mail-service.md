---
title: Definições de SMTP para o Microsoft 365 de correio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813979"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Definições de SMTP para o Microsoft 365 de correio

Estas são as definições SMTP para os serviços Microsoft 365 correio:

**Servidor:** smtp.office365.com </br>
**Porta:** 587 </br>
**Encriptação:** A versão STARTTLS (apenas é suportada a versão TLS 1.2). Certifique-se de que a sua aplicação ou dispositivo suporta TLS 1.2) </br>
**Nome de Utilizador:** o Office 365 Endereço da Conta (por exemplo, example@yourdomain.com) </br>
**Palavra-passe:** a sua palavra Office 365-passe </br>
**Autenticação:** obrigatório </br>
**Limites de Envio:** 10.000 E-mails por dia </br>

Para definições POP e IMAP, consulte [Definições de POP, IMAP e SMTP.](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353)
 
Para saber mais sobre as suas opções de reencanha e-mail com o Microsoft 365 e os passos, consulte Como configurar uma aplicação ou dispositivo [multifunções](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)para enviar e-mails através do Microsoft 365 ou Office 365 .