---
title: Требования к перераспределению для управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Узнайте, как можно перераспределить сборки управляемого API EWS с приложением.
ms.openlocfilehash: e64b4cdb8938caa819ba30621112a25946ef0424
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463827"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a><span data-ttu-id="48e46-103">Требования к перераспределению для управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="48e46-103">Redistribution requirements for the EWS Managed API</span></span>

<span data-ttu-id="48e46-104">Узнайте, как можно перераспределить сборки управляемого API EWS с приложением.</span><span class="sxs-lookup"><span data-stu-id="48e46-104">Find out how you can redistribute the EWS Managed API assemblies with your application.</span></span>
  
<span data-ttu-id="48e46-105">При проектировании приложения управляемого API EWS вы также захотите решить, как будет выпустить его для пользователей.</span><span class="sxs-lookup"><span data-stu-id="48e46-105">As you design your EWS Managed API application, you'll also want to consider how you will release it to your users.</span></span> 
  
## <a name="redistributing-your-ews-managed-api-application"></a><span data-ttu-id="48e46-106">Распространение приложения управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="48e46-106">Redistributing your EWS Managed API application</span></span>

<span data-ttu-id="48e46-107">Если ваше приложение не размещается на сервере Exchange Server, вам потребуется перераспределить сборки управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="48e46-107">Unless your application is located on the Exchange server, you will need to redistribute the EWS Managed API assemblies.</span></span> <span data-ttu-id="48e46-108">Загрузка управляемого API EWS содержит две сборки, которые можно перераспределить: Microsoft. Exchange. WebServices. dll и Microsoft. Exchange. WebServices. auth. dll.</span><span class="sxs-lookup"><span data-stu-id="48e46-108">The EWS Managed API download contains two assemblies that you can redistribute: Microsoft.Exchange.WebServices.dll and Microsoft.Exchange.WebServices.Auth.dll.</span></span> <span data-ttu-id="48e46-109">Когда вы разрабатываете приложение для управляемого API EWS, учитывайте следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="48e46-109">Keep the following information in mind when you design how you will release your EWS Managed API application:</span></span>
  
- <span data-ttu-id="48e46-110">Управляемый API EWS был разработан таким образом, чтобы его можно было скачать и распространить вместе с приложением, предназначенным для сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="48e46-110">The EWS Managed API was designed such that you can download it and distribute it with your application that targets an Exchange server.</span></span> <span data-ttu-id="48e46-111">Кроме того, приложение может скачать управляемый API EWS.</span><span class="sxs-lookup"><span data-stu-id="48e46-111">Alternatively, your application can download the EWS Managed API.</span></span>
    
- <span data-ttu-id="48e46-112">Вы можете использовать управляемый API EWS для обмена данными с сервером Exchange, на котором работает Exchange Online, Exchange Online в составе Office 365, или локальной версией Exchange, начиная с Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="48e46-112">You can use the EWS Managed API to communicate with an Exchange server running Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2007.</span></span>
    
- <span data-ttu-id="48e46-113">В версиях управляемого API EWS, начиная с версии 2,1, вы можете установить API в глобальном кэше сборок (GAC).</span><span class="sxs-lookup"><span data-stu-id="48e46-113">In versions of the EWS Managed API starting with version 2.1, you can install the API in the Global Assembly Cache (GAC).</span></span> <span data-ttu-id="48e46-114">MSI автоматически добавит библиотеку DLL в глобальный кэш сборок и будет доступна на уровне компьютера, а не на уровне пользователя.</span><span class="sxs-lookup"><span data-stu-id="48e46-114">The MSI will automatically add the DLL to the GAC and will be accessible on per computer basis, not on a per user basis.</span></span>
    
<span data-ttu-id="48e46-115">Условия лицензии включены в загрузку управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="48e46-115">The license terms are included in the EWS Managed API download.</span></span> <span data-ttu-id="48e46-116">Ознакомьтесь с условиями предоставления достоверных сведений о том, что можно сделать с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="48e46-116">Review the terms for the authoritative information about what you can do with the EWS Managed API.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="48e46-117">См. также</span><span class="sxs-lookup"><span data-stu-id="48e46-117">See also</span></span>


- [<span data-ttu-id="48e46-118">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="48e46-118">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="48e46-119">Управляемый API EWS (Загрузка)</span><span class="sxs-lookup"><span data-stu-id="48e46-119">EWS Managed API (download)</span></span>](https://aka.ms/ews-managed-api-readme)
    

