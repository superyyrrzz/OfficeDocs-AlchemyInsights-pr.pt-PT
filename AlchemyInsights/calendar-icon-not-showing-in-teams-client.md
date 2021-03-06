---
title: O ícone do Calendário não é apresentado no cliente do Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932198"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>O ícone do Calendário não é apresentado no cliente do Teams

O separador Calendário no Teams necessita de acesso a uma caixa de correio do Exchange através dos Serviços Web Exchange. A caixa de correio do Exchange pode estar Online ou No Local. Para utilizadores Online que não vejam o separador Calendário, certifique-se de que [têm licença para uma caixa de correio Exchange Online e que a caixa de correio está ativada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Se o utilizador tiver uma caixa de correio válida no Exchange Online, mas ainda não conseguir ver o separador Calendário, poderá estar a ter um problema de rede. Utilize o [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) e execute os **Testes de Conectividade dos Serviços Web do Microsoft Exchange** para o utilizador afetado.

Por último, consulte as [Políticas de configuração de aplicações nas Aplicações do Teams](https://admin.teams.microsoft.com/policies/app-setup) para garantir que a aplicação Calendário não foi removida da política aplicada ao utilizador (provavelmente a **Global (predefinição da organização)**.

Se os seus utilizadores estiverem alojados No Local, precisa de confirmar que a sua Configuração híbrida tem bom estado de funcionamento. Utilize o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para resolver problemas.

Tenha em conta que o [Teams necessita do Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
