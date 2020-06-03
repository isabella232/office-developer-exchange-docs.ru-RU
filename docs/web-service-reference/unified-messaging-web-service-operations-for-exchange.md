---
title: Операции веб-службы единой системы обмена сообщениями для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: d92455bd-24e8-4255-9f93-2bdeff00d42d
description: Справочные сведения по операциям веб-службы единой системы обмена сообщениями в Exchange.
ms.openlocfilehash: b13ca2fbc44846db0bc98b3961916ba5d0872310
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529716"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="f4ed9-103">Операции веб-службы единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="f4ed9-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="f4ed9-104">Справочные сведения по операциям веб-службы единой системы обмена сообщениями в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4ed9-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="f4ed9-105">Веб-служба единой системы обмена сообщениями предоставляет множество операций, которые позволяют клиентским приложениям считывать и изменять свойства единой системы обмена сообщениями, воспроизводящие голосовые сообщения, записывать приветствия и диктовать элементы почтовых ящиков телефонным устройствам.</span><span class="sxs-lookup"><span data-stu-id="f4ed9-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="f4ed9-106">В статьях этого раздела представлены сведения о общей структуре запросов и ответных сообщений для операций.</span><span class="sxs-lookup"><span data-stu-id="f4ed9-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="f4ed9-107">В этих статьях представлены примеры, демонстрирующие распространенные структуры сообщений.</span><span class="sxs-lookup"><span data-stu-id="f4ed9-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="f4ed9-108">Вы можете использовать эти примеры для получения сведений о том, что можно делать с запросом веб-службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f4ed9-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f4ed9-109">Для версий Exchange, начинающихся с Exchange 2010, рекомендуется использовать операции единой системы обмена сообщениями, доступные в [веб-службах Exchange (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) , а не в веб-службе единой системы обмена сообщениями по следующим причинам:</span><span class="sxs-lookup"><span data-stu-id="f4ed9-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons:</span></span> 
> - <span data-ttu-id="f4ed9-110">Функции единой системы обмена сообщениями на основе EWS имеют поддержку первого класса в управляемом API EWS.</span><span class="sxs-lookup"><span data-stu-id="f4ed9-110">The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="f4ed9-111">В версиях Exchange, начиная с Exchange 2010, новые функции единой системы обмена сообщениями добавляются в EWS, но не в веб-службу единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f4ed9-111">In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="f4ed9-112">В этой статье</span><span class="sxs-lookup"><span data-stu-id="f4ed9-112">In this section</span></span>
<span data-ttu-id="f4ed9-113"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="f4ed9-113"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="f4ed9-114">Операция отключения (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-114">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)    
- [<span data-ttu-id="f4ed9-115">Операция GetCallInfo (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-115">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)   
- [<span data-ttu-id="f4ed9-116">Операция GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-116">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)   
- [<span data-ttu-id="f4ed9-117">Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-117">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)   
- [<span data-ttu-id="f4ed9-118">Операция PlayOnPhone (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-118">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)   
- [<span data-ttu-id="f4ed9-119">Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-119">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)   
- [<span data-ttu-id="f4ed9-120">Операция ResetPIN (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-120">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)   
- [<span data-ttu-id="f4ed9-121">Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-121">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [<span data-ttu-id="f4ed9-122">Операция SetOofStatus (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-122">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)    
- [<span data-ttu-id="f4ed9-123">Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-123">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)   
- [<span data-ttu-id="f4ed9-124">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f4ed9-124">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="f4ed9-125">См. также</span><span class="sxs-lookup"><span data-stu-id="f4ed9-125">See also</span></span>

- [<span data-ttu-id="f4ed9-126">Справочные материалы по веб-службе единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="f4ed9-126">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="f4ed9-127">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4ed9-127">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="f4ed9-128">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="f4ed9-128">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

