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
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a>Установка URL-адрес службы веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange

Найдите сведения о том, как задать URL-адрес службы веб-служб Exchange в приложении управляемый API веб-служб Exchange.
  
URL-адрес службы — это адрес, используемый Exchange для взаимодействия с веб-служб Exchange (EWS). После того как приложение управляемый API EWS имеет этот адрес и имеет соответствующие права доступа для [взаимодействия с веб-служб Exchange](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), он может выполнять вызовы в [класс ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). URL-адрес службы для локального сервера Exchange может выглядеть следующим образом. 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

Можно задать URL-адрес веб-служб Exchange в приложении двумя способами. Мы рекомендуем использовать [службы автообнаружения](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) для получения URL-адрес, так как в крупных лес серверов, можно изменить URL-адрес при переносе почтовых ящиков на другой сервер. Тем не менее так как вызов автообнаружения может занять некоторое время и замедляет работу приложения, если требуется внести несколько вызовов в короткий промежуток времени, может потребоваться кэша значение URL-адреса вы получите от службы автообнаружения и вручную задать URL-адрес службы веб-служб Exchange с помощью этой кэшированные ва значение. Это позволит улучшить производительность приложения; только что убедитесь, что использование службы автообнаружения для обновления вашего кэшированное значение периодически в случае значение изменяется на сервере. 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a>Установка URL-адрес службы веб-служб Exchange с помощью службы автообнаружения
<a name="bk_SetURLusingAutoDiscover"> </a>

Метод [AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) используется адрес электронной почты, чтобы задать конечную точку [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и позволяет приложению использовать все методы, включенных в **ExchangeService** прокси-классы. Следующем примере показано, как использовать метод **AutodiscoverURL** . 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a>Вручную задать URL-адрес службы Exchange
<a name="bk_SetURLmanually"> </a>

Приведенный ниже показано, как задать URL-адрес службы веб-служб Exchange с помощью значения из кэша. Перед этим убедитесь в том получить URL-адрес веб-служб Exchange с помощью службы автообнаружения.
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a>См. также

- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md)   
- [Настройка среды разработки приложений Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Управление доступом к веб-служб Exchange в Exchange](how-to-control-access-to-ews-in-exchange.md) 
- [Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [Использование службы автообнаружения для поиска точек подключения](how-to-use-autodiscover-to-find-connection-points.md)
    

