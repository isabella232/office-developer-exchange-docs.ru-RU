---
title: Требования к распространения для управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Узнайте, как можно распространять на сборки управляемого интерфейса API веб-служб Exchange с приложением.
ms.openlocfilehash: d8fc57c4a2b3ed7d6218aeeed0fe88c2d3e0fbe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761236"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a><span data-ttu-id="1b5d5-103">Требования к распространения для управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1b5d5-103">Redistribution requirements for the EWS Managed API</span></span>

<span data-ttu-id="1b5d5-104">Узнайте, как можно распространять на сборки управляемого интерфейса API веб-служб Exchange с приложением.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-104">Find out how you can redistribute the EWS Managed API assemblies with your application.</span></span>
  
<span data-ttu-id="1b5d5-105">При разработке приложения управляемый API веб-служб Exchange, необходимо также рассмотрим, как оно будет выпуска для пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-105">As you design your EWS Managed API application, you'll also want to consider how you will release it to your users.</span></span> 
  
## <a name="redistributing-your-ews-managed-api-application"></a><span data-ttu-id="1b5d5-106">Распространение приложения управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="1b5d5-106">Redistributing your EWS Managed API application</span></span>

<span data-ttu-id="1b5d5-107">Если приложение находится на сервере Exchange, необходимо будет распространять сборки управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-107">Unless your application is located on the Exchange server, you will need to redistribute the EWS Managed API assemblies.</span></span> <span data-ttu-id="1b5d5-108">Управляемый API EWS файл содержит две сборки, которые можно распространять: Microsoft.Exchange.WebServices.dll и Microsoft.Exchange.WebServices.Auth.dll.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-108">The EWS Managed API download contains two assemblies that you can redistribute: Microsoft.Exchange.WebServices.dll and Microsoft.Exchange.WebServices.Auth.dll.</span></span> <span data-ttu-id="1b5d5-109">При разработке будет освобождение управляемый API EWS приложения необходимо учитывайте следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="1b5d5-109">Keep the following information in mind when you design how you will release your EWS Managed API application:</span></span>
  
- <span data-ttu-id="1b5d5-110">Управляемый API веб-служб Exchange был разработан таким образом, можно загрузить и распространять с приложением, предназначенное для Exchange server.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-110">The EWS Managed API was designed such that you can download it and distribute it with your application that targets an Exchange server.</span></span> <span data-ttu-id="1b5d5-111">Кроме того приложение можно загрузить управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-111">Alternatively, your application can download the EWS Managed API.</span></span>
    
- <span data-ttu-id="1b5d5-112">Управляемый API веб-служб Exchange можно использовать для связи с сервером Exchange под управлением Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-112">You can use the EWS Managed API to communicate with an Exchange server running Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2007.</span></span>
    
- <span data-ttu-id="1b5d5-113">В версиях управляемый API EWS начиная с версии 2.1 вы можете установить API в глобальный кэш сборок (GAC).</span><span class="sxs-lookup"><span data-stu-id="1b5d5-113">In versions of the EWS Managed API starting with version 2.1, you can install the API in the Global Assembly Cache (GAC).</span></span> <span data-ttu-id="1b5d5-114">MSI-файла автоматическое добавление библиотеки DLL в глобальный кэш сборок и будут доступны для каждого компьютера, а не на уровне пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-114">The MSI will automatically add the DLL to the GAC and will be accessible on per computer basis, not on a per user basis.</span></span>
    
<span data-ttu-id="1b5d5-115">Условия лицензионного соглашения будут включены в пакет загрузки управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-115">The license terms are included in the EWS Managed API download.</span></span> <span data-ttu-id="1b5d5-116">Ознакомьтесь с условиями достоверные сведения о возможностях управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b5d5-116">Review the terms for the authoritative information about what you can do with the EWS Managed API.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1b5d5-117">См. также</span><span class="sxs-lookup"><span data-stu-id="1b5d5-117">See also</span></span>


- [<span data-ttu-id="1b5d5-118">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="1b5d5-118">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="1b5d5-119">Управляемый API EWS (файл для загрузки)</span><span class="sxs-lookup"><span data-stu-id="1b5d5-119">EWS Managed API (download)</span></span>](http://aka.ms/ews-managed-api-readme)
    

