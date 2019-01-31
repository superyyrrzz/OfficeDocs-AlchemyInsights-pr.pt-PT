---
title: Políticas de retenção no Centro de administração do Exchange não funciona
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6c69511f6bcdad5793cd2473a20a2d168d2ac260
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660718"
---
 <span data-ttu-id="e5afa-102">**Problema:** Recentemente criados ou políticas de retenção actualizado no Centro de administração do Exchange não estão a aplicar às caixas de correio ou itens não são movidos para a caixa de correio do arquivo ou eliminadas.</span><span class="sxs-lookup"><span data-stu-id="e5afa-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="e5afa-103">**Causas raiz:**</span><span class="sxs-lookup"><span data-stu-id="e5afa-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="e5afa-p101">Isto pode ser porque o **Assistente da pasta gerida** não processou caixa de correio do utilizador. O Managed Assistente da pasta tenta processar cada caixa de correio na sua organização baseada na nuvem em sete dias. Se alterar um código de retenção ou aplicar uma política de retenção diferente a uma caixa de correio, pode esperar até que a pasta Assist geridos processa a caixa de correio ou pode executar o cmdlet Start-ManagedFolderAssistant para iniciar o Managed Assistente da pasta para processar um específico caixa de correio. Executar este cmdlet é útil para testar ou resolver problemas de definições de etiqueta de retenção ou de uma política de retenção. Para mais informações, visite a [executar o Managed Assistente da pasta](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="e5afa-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="e5afa-109">**Solução:** Execute o seguinte comando para iniciar o Managed Assistente da pasta para uma caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="e5afa-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="e5afa-p102">Isto também pode ser ocorrer se **RetentionHold** tiver sido **activada** a caixa de correio. Se a caixa de correio tiver sido colocada sobre uma RetentionHold, a política de retenção sobre a caixa de correio não será processada durante esse período. Para mais informações sobre sobre consulte de definição RetentionHold: [Mantenha de retenção de caixa de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="e5afa-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="e5afa-113">**Solução:**</span><span class="sxs-lookup"><span data-stu-id="e5afa-113">**Solution:**</span></span>
    
  - <span data-ttu-id="e5afa-114">Verifique o estado da definição da caixa de correio específica no [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)RetentionHold:</span><span class="sxs-lookup"><span data-stu-id="e5afa-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="e5afa-115">Execute o seguinte comando para **desactivar a** RetentionHold numa caixa de correio específica:</span><span class="sxs-lookup"><span data-stu-id="e5afa-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="e5afa-116">Agora, volte a executar a Assistente de pasta geridos:</span><span class="sxs-lookup"><span data-stu-id="e5afa-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="e5afa-117">**Nota:** Se uma caixa de correio for inferior a 10 MB, o Managed Assistente da pasta não irá automaticamente processar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e5afa-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  
