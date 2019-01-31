---
title: Resolver problemas relacionados com a inscrição de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655894"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="a217b-102">Resolver problemas relacionados com a inscrição de dispositivos Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a217b-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="a217b-103">Reveja os recursos listados abaixo para resolver o problema agora.</span><span class="sxs-lookup"><span data-stu-id="a217b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a217b-104">Alguns problemas comuns e passos de resolução:</span><span class="sxs-lookup"><span data-stu-id="a217b-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="a217b-p101">**Dispositivo não encriptados erro no Portal da empresa:** Versões mais recentes do Android, particularmente começando v 7.0, exigem uma palavra-passe de arranque para se certificar de que o dispositivo está totalmente encriptado. São soluções comuns activar um pin de arranque ou encriptar totalmente o dispositivo. Reveja [Este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a217b-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="a217b-p102">**Falham a verificação com o serviço de Intune ou como "Unhealthy" na consola de administração do Intune:** Alguns 4.4 Samsung e 5.5 dispositivos não podem verificar no serviço. Existem 3 soluções possíveis para este problema:</span><span class="sxs-lookup"><span data-stu-id="a217b-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="a217b-110">Abra manualmente a aplicação de Portal da empresa de Intune, que iniciará automaticamente uma sincronização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a217b-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="a217b-111">Actualize o dispositivo para Android 6.0 ou superior.</span><span class="sxs-lookup"><span data-stu-id="a217b-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="a217b-p103">Desactive Gestor inteligentes Samsung da gestão do Portal da empresa de Intune. Reveja [Este documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre estes problemas e resoluções.</span><span class="sxs-lookup"><span data-stu-id="a217b-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="a217b-p104">**Tipo de licença de utilizador inválido** ou **erro de utilizador nome não reconhecido:** o utilizador tem de ser atribuída uma licença de Intune ou EMS. Reveja estes documentos para atribuir uma licença através de: centro Admin do Office ou Azure portal.</span><span class="sxs-lookup"><span data-stu-id="a217b-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="a217b-116">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="a217b-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a217b-p105">Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Reveja [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="a217b-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="a217b-119">Reveja [Este documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) para uma lista de erros comuns que impedem a inscrição e resoluções para cada um.</span><span class="sxs-lookup"><span data-stu-id="a217b-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="a217b-120">[Obter informações sobre como inscrever-se dispositivos Android no Intune da Microsoft](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="a217b-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    
