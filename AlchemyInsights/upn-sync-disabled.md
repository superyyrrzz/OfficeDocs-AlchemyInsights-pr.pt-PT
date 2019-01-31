---
title: Sincronização UPN desactivada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657982"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="e85d8-102">Sincronização UPN desactivada</span><span class="sxs-lookup"><span data-stu-id="e85d8-102">UPN sync disabled</span></span>

<span data-ttu-id="e85d8-103">Se iniciar a sincronização com AD Azure antes de 30 de Março de 2016, execute o cmdlet Azure AD PowerShell seguinte para activar a correspondência de software de UPN para a sua organização apenas:</span><span class="sxs-lookup"><span data-stu-id="e85d8-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="e85d8-104">**Conjunto-MsolDirSyncFeature-funcionalidade EnableSoftMatchOnUpn-activar $True**</span><span class="sxs-lookup"><span data-stu-id="e85d8-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="e85d8-105">Correspondência de software de UPN é automaticamente activada para organizações que iniciou a sincronização com AD Azure em ou após 30 de Março de 2016.</span><span class="sxs-lookup"><span data-stu-id="e85d8-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="e85d8-106">Para obter mais informações sobre como activar a correspondência com software UPN e outras funcionalidades de sincronização, consulte [funcionalidades de suporte de sincronização Azure AD ligar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="e85d8-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  
