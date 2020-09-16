---
title: Notificações no Yammer
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
- "9002878"
- "5480"
ms.openlocfilehash: c1fbeea7bf4269e90e52cf5c129e904c99714926
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662804"
---
# <a name="notifications-in-yammer"></a>Notificações no Yammer

Para alertá-lo para novas atividades em conversas relevantes, o [Yammer envia notificações](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) quer por e-mail, quer por notificações push (se usar o Yammer no seu dispositivo móvel). Por predefinição, o Yammer envia notificações para diversos tipos de atividade na sua rede. Os utilizadores podem atualizar as suas definições de e-mail através do site do Yammer, e as notificações push são configuradas através da aplicação móvel. 

O Yammer adicionou suporte para [E-mails interativos no Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Alguns e-mails (cópia da mensagem) tornar-se-ão interativos no Outlook na Web. Uma atualização futura trará esta funcionalidade para outras versões do Outlook.

**Tipos de notificações no Yammer**

- E-mails (atualizações de um grupo, convites para grupos, quando recebe uma mensagem na sua caixa de entrada, etc.)
- Notificações push (Enviadas para dispositivos móveis quando recebe uma menção, quando recebe uma mensagem na sua caixa de entrada, etc.)
- Pop-ups no ambiente de trabalho (Quando tiver a aplicação Yammer para ambiente de trabalho instalada, esta apresentará notificações aos utilizadores, chamadas notificações “toast”.)
- Notificações de campainha (Dentro do site Yammer, os utilizadores verão notificações para diferentes eventos. Estas notificações poderão nem sempre estar associadas a uma mensagem de correio eletrónico ou a uma notificação push.)

Estão disponíveis mais [informações detalhadas sobre notificações](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Gerir notificações**

Os utilizadores devem gerir as suas próprias notificações. Existe informação disponível sobre [como ativar e desativar as notificações por e-mail e notificações móveis do Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Não é possível que os administradores desativem todas as notificações, ou que controlem as notificações no lugar dos utilizadores. Os administradores podem [controlar o logótipo incluído nos e-mails e se os utilizadores precisam ou não de confirmar as mensagens](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) publicadas por e-mail.

**Notificações de e-mail enviadas a muitos utilizadores na sua organização**

Por vezes, uma única notificação de e-mail será enviada pelo Yammer e recebida por muitos mais utilizadores na sua organização do que o esperado. Isto acontece quando uma lista de distribuição, ou outro tipo de endereço de e-mail não individual, é adicionado ao Yammer. O Yammer não sabe, em todos os casos, se um endereço de e-mail pertence a um único utilizador, ou se é um endereço de e-mail que fará com que uma mensagem de correio eletrónico seja entregue a muitos destinatários. Quando este problema ocorrer, deve tomar medidas para [suspender (desativar) o utilizador inválido que tenha esse endereço de e-mail](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) no Yammer. 

Para reduzir a probabilidade de este problema ocorrer, deve:

1. [Impor a identidade do Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) para o Yammer.
2. Bloquear remetentes externos de enviar e-mails para a sua organização ou limitar os remetentes a uma lista aprovada.

Se este problema ocorrer:

1. Identifique o destinatário do e-mail, que deve coincidir com o utilizador no Yammer. Por exemplo, all-in-sales@fabrikam.com é um DL para todos os vendedores. Este DL seria identificável a partir do e-mail Yammer recebido pelos utilizadores.
2. Utilize a [funcionalidade desativar (suspender) na Administração de Rede](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) para suspender o utilizador que tenha o endereço de e-mail all-in-sales@fabrikam.com. A suspensão pode ser revertida, por isso é mais segura do que a eliminação. A eliminação do utilizador acontecerá automaticamente após 90 dias.
3. Opcionalmente, reveja a [Exportação de Utilizadores](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) para identificar outros endereços de e-mail de não utilizadores que devam ser suspensos.
