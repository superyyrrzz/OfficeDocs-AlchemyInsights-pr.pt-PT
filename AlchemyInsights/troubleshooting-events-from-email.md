---
title: Eventos de resolução de problemas a partir de e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569407"
---
# <a name="troubleshooting-events-from-email"></a>Eventos de resolução de problemas a partir de e-mail

1. Verifique se a funcionalidade está ativada para a caixa de correio: **Get-EventsFromEmailConfiguration -Identidade <mailbox> **

2. Em seguida, veja os registos 'Eventos do Email' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Nos registos 'Eventos do Email', encontre o InternetMessageId que corresponda ao item na caixa de correio.  

4. O TrustScore determina se o artigo é adicionado ou não. Os eventos só serão adicionados se o TrustScore = "Trusted".

O TrustScore é determinado pelas propriedades SPF, Dkim ou Dmarc, que estão no Cabeçalho de Mensagem.

Para ver estas propriedades:

**Perspetivas de Ambiente de Trabalho**

- Abra o item
- File -> Properties -> Cabeçalhos de Internet

ou

**MFCMapi**

- Navegue para o item na caixa de entrada
- Procure por PR_TRANSPORT_MESSAGE_HEADERS_W

Estas propriedades são determinadas e registadas durante o transporte e encaminhamento. Para uma resolução de problemas, poderá ter de acompanhar o Apoio ao Transporte sobre as falhas em SPF, DKIM e.ou DMARC.