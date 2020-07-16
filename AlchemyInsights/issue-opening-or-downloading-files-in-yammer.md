---
title: Emissão de abrir ou descarregar ficheiros em Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148337"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Emissão de abrir ou descarregar ficheiros em Yammer

A Classic Yammer suporta múltiplas opções para uploads de ficheiros para mensagens e grupos. Dependendo da configuração da rede, os ficheiros predefinição para armazenamento no SharePoint.

O selecionador de ficheiros em novo Yammer ainda não suporta todas as opções disponíveis no clássico Yammer. Uma futura atualização irá adicionar funcionalidades adicionais. Para obter mais informações, consulte [anexar um ficheiro ou imagem a um post de conversação Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Incapaz de abrir ou descarregar um ficheiro**  

Um ficheiro pode ser enviado para o Yammer, mas também estar ligado a um ficheiro no SharePoint Online. Para resolver problemas, primeiro tem de determinar a localização do ficheiro. Se o ficheiro tiver sido enviado para o Yammer, terá uma URL de yammer.com. Certifique-se de que os URLs e endereços IP necessários estão desbloqueados. Para obter mais informações, consulte o post de blog [Usando endereços IP codificados para Yammer não é recomendado](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Verifique se um utilizador que também é administrador global pode descarregar o ficheiro. Se o ficheiro for privado, poderá ter de utilizar o Modo de Conteúdo Privado. Para obter mais informações, consulte então [monitorize o conteúdo privado em Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Hóspedes e ficheiros ao nível da rede Yammer no SharePoint Online**  

[Os hóspedes de nível de rede em Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) não usam Azure AD B2B e são internos ao serviço Yammer, por isso não podem aceder aos ficheiros Yammer armazenados no SharePoint. Crie um utilizador AAD B2B externo que possa aceder a bibliotecas documentais no SharePoint Online utilizando essa identidade. Para obter informações sobre o futuro suporte de hóspedes Azure AD B2B em Yammer, consulte [suporte de clientes Business-to-Business (B2B) em Yammer Preview - Termos do Cliente e FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).