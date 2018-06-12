---
title: Агенты транспорта в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 36d63aa6-1b72-4670-b5c3-da685f3017cb
description: Сведения о агенты транспорта в Exchange 2013.
ms.openlocfilehash: 1a28ae79e2a7e338ddd6cb1f6961dd14a980b56e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761319"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="17756-103">Агенты транспорта в Exchange</span><span class="sxs-lookup"><span data-stu-id="17756-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="17756-104">Exchange 2013 предоставляет библиотеки классов, которые поддерживают расширение поведения транспорта Exchange и включить чтение, запись и преобразования типов контента.</span><span class="sxs-lookup"><span data-stu-id="17756-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="17756-105">Можно использовать эти классы для создания приложений транспорта Exchange, чтение, запись и обрабатывать сообщения в транспортном конвейере.</span><span class="sxs-lookup"><span data-stu-id="17756-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="17756-106">Что нужно знать о агенты транспорта</span><span class="sxs-lookup"><span data-stu-id="17756-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="17756-107">Если вам интересно о...</span><span class="sxs-lookup"><span data-stu-id="17756-107">If you're wondering about…</span></span>|<span data-ttu-id="17756-108">Прочтите это</span><span class="sxs-lookup"><span data-stu-id="17756-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="17756-109">Availability</span><span class="sxs-lookup"><span data-stu-id="17756-109">Availability</span></span>  <br/> |<span data-ttu-id="17756-110">Агенты транспорта, доступные в версии Exchange, начиная с Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="17756-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="17756-111">Агенты транспорта не поддерживаются в Office 365 и Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="17756-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="17756-112">Remote usage</span><span class="sxs-lookup"><span data-stu-id="17756-112">Remote usage</span></span>  <br/> |<span data-ttu-id="17756-113">Агенты транспорта, выполните на сервере Exchange и не поддерживает удаленное использование.</span><span class="sxs-lookup"><span data-stu-id="17756-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="17756-114">Поддерживаемые языки</span><span class="sxs-lookup"><span data-stu-id="17756-114">Languages supported</span></span>  <br/> |<span data-ttu-id="17756-115">Можно использовать любой язык .NET Framework для работы с агенты транспорта.</span><span class="sxs-lookup"><span data-stu-id="17756-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="17756-116">Доступные инструменты для тестирования и отладки</span><span class="sxs-lookup"><span data-stu-id="17756-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="17756-117">Использование версий Visual Studio, начиная с помощью Visual Studio 2012 для отладки агенты транспорта.</span><span class="sxs-lookup"><span data-stu-id="17756-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="17756-118">Deployment methods</span><span class="sxs-lookup"><span data-stu-id="17756-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="17756-119">С помощью сценария [Командной консоли Exchange](../management/exchange-management-shell.md) можно установить приложения агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="17756-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="17756-120">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="17756-120">In this section</span></span>

- [<span data-ttu-id="17756-121">Агент транспорта новые и обновленные интерфейсы API в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="17756-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="17756-122">Транспорта агента образцы кода для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="17756-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="17756-123">Транспорта концепции агентов в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="17756-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="17756-124">Чтение и изменение сообщений в транспортный конвейер Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="17756-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="17756-125">Создание агенты транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="17756-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="17756-126">Справочник по агента транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="17756-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="17756-127">См. также</span><span class="sxs-lookup"><span data-stu-id="17756-127">See also</span></span>

- [<span data-ttu-id="17756-128">Exchange Online и Exchange (en)</span><span class="sxs-lookup"><span data-stu-id="17756-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="17756-129">Сведения об управляемом API EWS, EWS и веб-службах в Exchange</span><span class="sxs-lookup"><span data-stu-id="17756-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="17756-130">Резервное копирование и восстановление для Exchange</span><span class="sxs-lookup"><span data-stu-id="17756-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

