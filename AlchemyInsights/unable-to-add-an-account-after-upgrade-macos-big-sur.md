---
title: Não é possível adicionar uma conta após atualizar para o macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506753"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Não é possível adicionar uma conta após atualizar para o macOS 11.6 Big Sur

Após atualizar para o macOS 11.6, a sua conta escolar ou escolar do OneDrive ou a sua conta escolar ou pessoal do OneDrive poderá não aparecer na sua lista de contas e poderá não conseguir iniciar sessão numa segunda conta a partir da aplicação.

Foi desenvolvida uma correção para este problema. Primeiro, determine se está a executar a versão atual da App Store ou OneDrive:

- Selecione a nuvem OneDrive de Menus na barra de menus > **Ajuda & Definições**  >  **Preferências**  >  **Sobre**. Se o número da versão não incluir **(A standalone),** significa que tem a versão da App Store do produto.

Se estiver a utilizar a versão autógrafa do OneDrive, reinicie o seu aparelho e faça OneDrive atualizações automáticas para uma compor onde este problema foi resolvido. Se quiser instalar a composição manualmente, transfira este ficheiro [do.zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), deszipe o ficheiro e copie a aplicação OneDrive para a pasta Aplicações (substituindo a aplicação OneDrive existente).

Se estiver a utilizar a versão da App Store, considere instalar a versão atual do OneDrive. Esta versão funciona da mesma forma que a versão da App Store, mas permite que a Microsoft ofereça atualizações mais rapidamente aos utilizadores e liga-os a uma versão que inclui a correção para este problema.

1. Transfira a versão atual [do OneDrive que inclui a correção.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Deszipe o ficheiro e copie a OneDrive para a pasta Aplicações (substituindo a aplicação OneDrive existente).

Se precisar de utilizar a versão da App Store, aguarde até que a App Store liberte uma versão da aplicação que inclua a correção. Infelizmente, a Microsoft não consegue comunicar uma data estimada para o lançamento de uma versão fixa a partir da App Store.


