---
title: Trabalhar com bibliotecas de autenticação
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036872"
---
# <a name="working-with-authentication-libraries"></a>Trabalhar com bibliotecas de autenticação

Para resolver o problema da Biblioteca de Autenticação do Microsoft (MSAL), execute os seguintes passos recomendados:

1. **Trabalhar com a MSAL**: [Bibliotecas de autenticação da plataforma de identidade microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - Este artigo mostra o suporte da Microsoft Authentication Library para vários tipos de aplicações. Inclui links para código fonte de biblioteca; onde obter o pacote para o projeto da sua aplicação; e se a biblioteca suporta o acesso ao utilizador (autenticação), o acesso a APIs web protegidas (autorização), ou ambos.

2. **Resolução de problemas Autenticação**: O MSAL suporta vários fluxos de autenticação para utilização em diferentes cenários de aplicação. Dependendo da forma como a aplicação do seu cliente é construída, o MSAL pode utilizar um ou mais dos fluxos de autenticação suportados pela plataforma de identidade microsoft. Estes fluxos podem produzir vários tipos de fichas e códigos de autorização, e requerem diferentes fichas para fazê-los funcionar.

3. **Tokens de acesso**: [Fichas de acesso à plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Saiba como a sua API pode validar e utilizar as reclamações dentro de um token de acesso. Toda a documentação deste artigo, exceto quando anotado, aplica-se apenas a fichas emitidas para APIs que tenha registado. Não se aplica a fichas emitidas para APIs detidas pela Microsoft, nem esses tokens podem ser usados para validar como a plataforma de identidade da Microsoft emitirá fichas para uma API que cria.

**Fim do suporte para a Biblioteca de Autenticação do Diretório Ativo Azure (ADAL)**

- **A partir de 30 de junho de 2020,** deixaremos de adicionar novas funcionalidades ao ADAL e ao Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.
- **A partir de 30 de junho de 2022,** terminaremos o suporte ao ADAL e ao Azure AD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.
- As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não *receberão qualquer suporte técnico ou atualizações de segurança.*
- As aplicações que utilizam o Azure AD Graph após este tempo podem deixar de receber respostas do ponto final do Azure AD Graph.

**Migração ADAL**

- Recomendamos a atualização ao MSAL, que tem as mais recentes funcionalidades e atualizações de segurança.
- Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está em processo de migrar as suas apps para o MSAL até ao fim do prazo de suporte, garantindo que beneficiará da segurança contínua da MSAL e das melhorias de funcionalidades.

1. [Leia as FAQ ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba como migrar aplicações por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Se, depois de ler o guia para a plataforma da sua aplicação, tiver perguntas adicionais, pode publicar no [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) com a etiqueta [azure-ad-adal-depreciação] ou abrir um problema no repositório GitHub da biblioteca. Consulte a secção [de Línguas e Quadros](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) do artigo **de visão geral** do MSAL para obter links para o repo de cada biblioteca.
4. **Se precisar de ajuda para entender quais das suas aplicações usam ADAL,** recomendamos que reveja todo o código fonte das suas apps. Se aplicável, contacte qualquer fornecedor de software independente (ISVs) ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.







