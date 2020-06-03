---
title: Настройка URL-адреса службы EWS с помощью управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: Найдите сведения о том, как настроить URL-адрес службы EWS в приложении управляемого API EWS.
localization_priority: Priority
ms.openlocfilehash: 5ba79b48d4eb4fec62110448c5924de16b67ce10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456749"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a>Настройка URL-адреса службы EWS с помощью управляемого API EWS

Найдите сведения о том, как настроить URL-адрес службы EWS в приложении управляемого API EWS.
  
URL-адрес службы — это адрес, который Exchange использует для обмена данными с веб-службами Exchange (EWS). После того, как приложение управляемого API EWS использует этот адрес и имеет соответствующий доступ для [связи с EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), он может совершать вызовы в [класс ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). URL-адрес службы для локального сервера Exchange может выглядеть следующим образом. 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

URL-адрес EWS в приложении можно задать несколькими способами. Рекомендуется использовать [службу автообнаружения](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) для получения URL-адреса, так как в большом лесу серверов URL-адрес может измениться при переносе почтового ящика на другой сервер. Однако так как вызов автообнаружения может занять некоторое время и может замедлить работу приложения, если необходимо выполнить несколько вызовов в течение короткого периода времени, можно кэшировать значение URL-адреса, полученное с помощью автообнаружения, и вручную задать URL-адрес службы EWS с этим кэшированным значением. Это повысит производительность приложения; просто убедитесь, что вы используете функцию автообнаружения для периодического обновления кэшированного значения, если на сервере изменяется значение. 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a>Настройка URL-адреса службы EWS с помощью службы автообнаружения
<a name="bk_SetURLusingAutoDiscover"> </a>

Метод [AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) использует адрес электронной почты для установки конечной точки [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и позволяет приложению использовать любые методы, включенные в прокси-классы **ExchangeService** . В приведенном ниже примере показано, как использовать метод **AutodiscoverURL** . 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a>Настройка URL-адреса службы Exchange вручную
<a name="bk_SetURLmanually"> </a>

В приведенном ниже примере показано, как задать URL-адрес службы EWS с помощью кэшированного значения. Перед выполнением этой операции убедитесь, что для получения URL-адреса веб-служб EWS используется служба автообнаружения.
  
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
- [Контроль доступа к EWS в Exchange](how-to-control-access-to-ews-in-exchange.md) 
- [Взаимодействие с EWS с помощью управляемого API EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [Поиск точек соединения с помощью службы автообнаружения](how-to-use-autodiscover-to-find-connection-points.md)
    

