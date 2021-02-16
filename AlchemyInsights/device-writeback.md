---
title: Writeback do dispositivo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256858"
---
# <a name="device-writeback"></a>Writeback do dispositivo

O Writeback do dispositivo é utilizado nos seguintes cenários:

- Ativar [o Windows Hello for Business utilizando a implementação híbrida do certificado trust](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Ativar o Acesso Condicional com base em dispositivos a aplicações protegidas ADFS (2012 R2 ou superior) (confianças de partes)

    > [!NOTE]
    > É necessária uma subscrição do Azure AD Premium para a gravação do dispositivo.

Isto fornece segurança adicional e garantia de que o acesso a aplicações é concedido apenas a dispositivos fidedignos. Para obter mais informações sobre o Acesso Condicional, consulte [o Risco de Gestão com Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) e [Configuração de Acesso Condicional utilizando o Registo do Dispositivo de Diretório Ativo Azure](https://docs.microsoft.com/azure/active-directory/devices/overview).

Para obter mais informações sobre a redução do dispositivo ativante para dispositivos, consulte [ativar a writeback do dispositivo](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
