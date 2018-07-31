---
title: Операции единой системы обмена сообщениями веб-службы для Exchange
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
description: Найдите справочные сведения для операции веб-службы единой системы обмена сообщениями в Exchange.
ms.openlocfilehash: bd86a4ab2de58e5f04a8d37f17196040bcf38b97
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354360"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="7147b-103">Операции единой системы обмена сообщениями веб-службы для Exchange</span><span class="sxs-lookup"><span data-stu-id="7147b-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="7147b-104">Найдите справочные сведения для операции веб-службы единой системы обмена сообщениями в Exchange.</span><span class="sxs-lookup"><span data-stu-id="7147b-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="7147b-105">Веб-службы единой системы обмена сообщениями предоставляет множество операций, которые позволяют приложениям клиента для чтения и изменения свойств единой системы обмена сообщениями, воспроизведение голосовых сообщений, запишите приветствия и диктуют необходимость элементы почтовых ящиков через устройства телефонии.</span><span class="sxs-lookup"><span data-stu-id="7147b-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="7147b-106">Статьи в этом разделе представлены сведения о Общая структура сообщения запроса и ответа для операций.</span><span class="sxs-lookup"><span data-stu-id="7147b-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="7147b-107">В этих статьях содержатся примеры, иллюстрирующие общим структурам сообщения.</span><span class="sxs-lookup"><span data-stu-id="7147b-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="7147b-108">Можно использовать эти примеры, чтобы узнать о возможностях запрос веб-службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="7147b-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7147b-109">Версии Exchange, начиная с Exchange 2010 рекомендуется использовать операций единой системы обмена сообщениями, доступные в [Веб-служб Exchange (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) вместо единой системы обмена сообщениями веб-службы, по следующим причинам:</span><span class="sxs-lookup"><span data-stu-id="7147b-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons:</span></span> 
> - <span data-ttu-id="7147b-110">Функции на основе веб-служб Exchange единой системы обмена сообщениями имеют поддержку в управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="7147b-110">The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="7147b-111">В версиях Exchange, начиная с Exchange 2010 добавляются новые возможности единой системы обмена сообщениями, веб-служб Exchange, но не к веб-службе единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="7147b-111">In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="7147b-112">В этой статье</span><span class="sxs-lookup"><span data-stu-id="7147b-112">In this section</span></span>
<span data-ttu-id="7147b-113"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="7147b-113"></span></span>

- [<span data-ttu-id="7147b-114">Операция Disconnect (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-114">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)    
- [<span data-ttu-id="7147b-115">Операция GetCallInfo (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-115">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)   
- [<span data-ttu-id="7147b-116">Операция GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-116">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)   
- [<span data-ttu-id="7147b-117">Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-117">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)   
- [<span data-ttu-id="7147b-118">Операция PlayOnPhone (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-118">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)   
- [<span data-ttu-id="7147b-119">Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-119">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)   
- [<span data-ttu-id="7147b-120">Операция ResetPIN (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-120">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)   
- [<span data-ttu-id="7147b-121">Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-121">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [<span data-ttu-id="7147b-122">Операция SetOofStatus (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-122">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)    
- [<span data-ttu-id="7147b-123">Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-123">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)   
- [<span data-ttu-id="7147b-124">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="7147b-124">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="7147b-125">См. также</span><span class="sxs-lookup"><span data-stu-id="7147b-125">See also</span></span>

- [<span data-ttu-id="7147b-126">Единой системы обмена сообщениями веб-службы ссылки для Exchange</span><span class="sxs-lookup"><span data-stu-id="7147b-126">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="7147b-127">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="7147b-127">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="7147b-128">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="7147b-128">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

