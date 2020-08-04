---
title: Questões relacionadas com a VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555230"
---
# <a name="vpn-related-issues"></a>Questões relacionadas com a VPN

A implementação bem sucedida da conectividade VPN para clientes MDM depende de um perfil implantado que reflita corretamente os requisitos da infraestrutura VPN. Para as definições apropriadas para as plataformas de clientes que está a investigar, consulte: 

[Windows 10 e Windows Holographic device configurações para adicionar ligações VPN usando Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Adicione definições VPN em dispositivos iOS e iPadOS no Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Configurações de dispositivos Android para configurar VPN em Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Adicione definições VPN em dispositivos macOS no Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Se o seu perfil VPN utilizar a autenticação baseada em certificados, certifique-se de que os perfis de certificado de base e de certificado de autenticação do cliente ligados ao perfil VPN são implementados com sucesso.

**Questões Comuns**

**Desloquei um perfil VPN para um dispositivo. A Intune está a mostrar que foi bem sucedida, mas o dispositivo não está a ligar-se à VPN.**

Um estado de sucesso significa que a Intune implementou o perfil com sucesso como configurado. No entanto, estas configurações podem não corresponder aos seus requisitos de rede e/ou autenticação. Reveja os registos no serviço de infraestrutura e autenticação (no servidor VPN e no servidor NPS/Radius) para obter mais detalhes sobre a tentativa de ligação. Poderá ter de trabalhar com a sua equipa de infraestruturas de rede, ou com o fornecedor de VPN de terceiros, para recolher e rever registos.

**Quando configurar uma VPN personalizada para iOS, a funcionalidade VPN por aplicação não é disponibilizada.**

A VPN por aplicação para dispositivos iOS no Intune está atualmente disponível para uma lista específica de fornecedores e parceiros, que também devem cumprir os pré-requisitos do certificado antes de configurar uma VPN por aplicação. Para obter mais informações, consulte [Configurar por aplicação Rede Privada Virtual (VPN) para dispositivos iOS/iPadOS no Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Para obter mais informações sobre todos os tipos de conexão VPN no Intune, consulte [criar perfis VPN para ligar aos servidores VPN no Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**IOS On Demand VPN não é desencadeando quando um domínio configurado é acedido**

Para testar as definições automáticas de VPN, defina os seguintes valores:

Quero fazer o seguinte: **Avaliar cada tentativa de ligação** 

Escolha se deve ligar: **Conecte-se se necessário**

Quando os utilizadores acedem a estes domínios: nome de **domínio-alvo** *domain name*

Se a configuração acima não for bem sucedida, adicione o seguinte elemento:

Quando este URL é inacessível, force a ligação da VPN: **BADURL**