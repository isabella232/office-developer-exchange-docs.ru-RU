---
title: Агенты транспорта в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 36d63aa6-1b72-4670-b5c3-da685f3017cb
description: Поиск сведений об агентах транспорта в Exchange 2013.
ms.openlocfilehash: 1a28ae79e2a7e338ddd6cb1f6961dd14a980b56e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761319"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="16210-103">Агенты транспорта в Exchange</span><span class="sxs-lookup"><span data-stu-id="16210-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="16210-104">Exchange 2013 предоставляет библиотеку классов, поддерживающих расширение режима транспорта Exchange и обеспечивающее возможность чтения, записи и преобразования типов контента.</span><span class="sxs-lookup"><span data-stu-id="16210-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="16210-105">Эти классы можно использовать для создания приложений транспорта Exchange, которые читают, пишут и обрабатывают сообщения в транспортном конвейере.</span><span class="sxs-lookup"><span data-stu-id="16210-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="16210-106">Что нужно знать об агентах транспорта</span><span class="sxs-lookup"><span data-stu-id="16210-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="16210-107">Если вас интересует...</span><span class="sxs-lookup"><span data-stu-id="16210-107">If you're wondering about…</span></span>|<span data-ttu-id="16210-108">Прочтите это</span><span class="sxs-lookup"><span data-stu-id="16210-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="16210-109">Доступность</span><span class="sxs-lookup"><span data-stu-id="16210-109">Availability</span></span>  <br/> |<span data-ttu-id="16210-110">Агенты транспорта доступны в версиях Exchange, начиная с Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="16210-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="16210-111">Агенты транспорта не поддерживаются в Office 365 или Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="16210-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="16210-112">Удаленное использование</span><span class="sxs-lookup"><span data-stu-id="16210-112">Remote usage</span></span>  <br/> |<span data-ttu-id="16210-113">Агенты транспорта выполняются на сервере Exchange Server и не поддерживают удаленное использование.</span><span class="sxs-lookup"><span data-stu-id="16210-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="16210-114">Поддерживаемые языки</span><span class="sxs-lookup"><span data-stu-id="16210-114">Languages supported</span></span>  <br/> |<span data-ttu-id="16210-115">Для работы с агентами транспорта можно использовать любой язык платформы .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="16210-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="16210-116">Доступные инструменты для тестирования и отладки</span><span class="sxs-lookup"><span data-stu-id="16210-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="16210-117">Используйте версии Visual Studio, начиная с Visual Studio 2012, для отладки агентов транспорта.</span><span class="sxs-lookup"><span data-stu-id="16210-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="16210-118">Методы развертывания</span><span class="sxs-lookup"><span data-stu-id="16210-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="16210-119">Приложения агента транспорта можно установить с помощью сценария [командной консоли Exchange](../management/exchange-management-shell.md) .</span><span class="sxs-lookup"><span data-stu-id="16210-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="16210-120">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="16210-120">In this section</span></span>

- [<span data-ttu-id="16210-121">Новые и обновленные API агента транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="16210-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="16210-122">Примеры кода агента транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="16210-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="16210-123">Основные понятия, связанные с агентами транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="16210-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="16210-124">Чтение и изменение сообщений в транспортном конвейере Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="16210-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="16210-125">Создание агентов транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="16210-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="16210-126">Справочник по агентам транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="16210-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="16210-127">См. также</span><span class="sxs-lookup"><span data-stu-id="16210-127">See also</span></span>

- [<span data-ttu-id="16210-128">Разработки для Exchange Online и Exchange</span><span class="sxs-lookup"><span data-stu-id="16210-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="16210-129">Сведения об управляемом API EWS, EWS и веб-службах в Exchange</span><span class="sxs-lookup"><span data-stu-id="16210-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="16210-130">Резервное копирование и восстановление для Exchange</span><span class="sxs-lookup"><span data-stu-id="16210-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

