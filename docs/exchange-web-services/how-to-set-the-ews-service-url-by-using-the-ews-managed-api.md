---
title: Установка URL-адрес службы веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: Найдите сведения о том, как задать URL-адрес службы веб-служб Exchange в приложении управляемый API веб-служб Exchange.
ms.openlocfilehash: e1a414f7c6f13bd61a58403c9d2be546c0226a69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761109"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a><span data-ttu-id="f0d7a-103">Установка URL-адрес службы веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="f0d7a-103">Set the EWS service URL by using the EWS Managed API</span></span>

<span data-ttu-id="f0d7a-104">Найдите сведения о том, как задать URL-адрес службы веб-служб Exchange в приложении управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-104">Find information about how to set the EWS service URL in your EWS Managed API application.</span></span>
  
<span data-ttu-id="f0d7a-105">URL-адрес службы — это адрес, используемый Exchange для взаимодействия с веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="f0d7a-105">The service URL is the address that Exchange uses to communicate with Exchange Web Services (EWS).</span></span> <span data-ttu-id="f0d7a-106">После того как приложение управляемый API EWS имеет этот адрес и имеет соответствующие права доступа для [взаимодействия с веб-служб Exchange](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), он может выполнять вызовы в [класс ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f0d7a-106">After your EWS Managed API application has this address, and has appropriate access to [communicate with EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), it can make calls to the [ExchangeService class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="f0d7a-107">URL-адрес службы для локального сервера Exchange может выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-107">The service URL for an on-premises Exchange server might look like the following.</span></span> 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

<span data-ttu-id="f0d7a-108">Можно задать URL-адрес веб-служб Exchange в приложении двумя способами.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-108">You can set the EWS URL in your application in a couple of ways.</span></span> <span data-ttu-id="f0d7a-109">Мы рекомендуем использовать [службы автообнаружения](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) для получения URL-адрес, так как в крупных лес серверов, можно изменить URL-адрес при переносе почтовых ящиков на другой сервер.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-109">We recommend that you use the [Autodiscover service](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) to get the URL because in a large forest of servers, the URL can change if the mailbox is migrated to another server.</span></span> <span data-ttu-id="f0d7a-110">Тем не менее так как вызов автообнаружения может занять некоторое время и замедляет работу приложения, если требуется внести несколько вызовов в короткий промежуток времени, может потребоваться кэша значение URL-адреса вы получите от службы автообнаружения и вручную задать URL-адрес службы веб-служб Exchange с помощью этой кэшированные ва значение.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-110">However, because calling Autodiscover can take some time and can slow down your application if you need to make multiple calls in a short period of time, you might want to cache the URL value you get from Autodiscover and manually set the EWS service URL with this cached value.</span></span> <span data-ttu-id="f0d7a-111">Это позволит улучшить производительность приложения; только что убедитесь, что использование службы автообнаружения для обновления вашего кэшированное значение периодически в случае значение изменяется на сервере.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-111">This will improve the performance of your application; just make sure that you use Autodiscover to update your cached value periodically in case the value changes on the server.</span></span> 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a><span data-ttu-id="f0d7a-112">Установка URL-адрес службы веб-служб Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="f0d7a-112">Set the EWS service URL by using the Autodiscover service</span></span>
<span data-ttu-id="f0d7a-113"><a name="bk_SetURLusingAutoDiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="f0d7a-113"></span></span>

<span data-ttu-id="f0d7a-114">Метод [AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) используется адрес электронной почты, чтобы задать конечную точку [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и позволяет приложению использовать все методы, включенных в **ExchangeService** прокси-классы.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-114">The [AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method uses the email address to set the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) endpoint and enables your application to use any methods included in the **ExchangeService** proxy classes.</span></span> <span data-ttu-id="f0d7a-115">Следующем примере показано, как использовать метод **AutodiscoverURL** .</span><span class="sxs-lookup"><span data-stu-id="f0d7a-115">The following example shows how to use the **AutodiscoverURL** method.</span></span> 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a><span data-ttu-id="f0d7a-116">Вручную задать URL-адрес службы Exchange</span><span class="sxs-lookup"><span data-stu-id="f0d7a-116">Set the Exchange service URL manually</span></span>
<span data-ttu-id="f0d7a-117"><a name="bk_SetURLmanually"> </a></span><span class="sxs-lookup"><span data-stu-id="f0d7a-117"></span></span>

<span data-ttu-id="f0d7a-118">Приведенный ниже показано, как задать URL-адрес службы веб-служб Exchange с помощью значения из кэша.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-118">The following example shows you how to set the EWS service URL by using a cached value.</span></span> <span data-ttu-id="f0d7a-119">Перед этим убедитесь в том получить URL-адрес веб-служб Exchange с помощью службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="f0d7a-119">Before you do this, make sure to use the Autodiscover service to get the EWS URL.</span></span>
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a><span data-ttu-id="f0d7a-120">См. также</span><span class="sxs-lookup"><span data-stu-id="f0d7a-120">See also</span></span>

- [<span data-ttu-id="f0d7a-121">Начало работы с клиентскими приложениями, использующими управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="f0d7a-121">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)   
- [<span data-ttu-id="f0d7a-122">Настройка среды разработки приложений Exchange</span><span class="sxs-lookup"><span data-stu-id="f0d7a-122">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="f0d7a-123">Управление доступом к веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f0d7a-123">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md) 
- [<span data-ttu-id="f0d7a-124">Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="f0d7a-124">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [<span data-ttu-id="f0d7a-125">Использование службы автообнаружения для поиска точек подключения</span><span class="sxs-lookup"><span data-stu-id="f0d7a-125">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    

