---
title: Операция ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Найдите сведения о веб-служб Exchange ConvertId операции.
ms.openlocfilehash: 5f1bcd8a9f0adc25b7c598ef10cc6bb139dfe02d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761826"
---
# <a name="convertid-operation"></a>Операция ConvertId

Найдите сведения о **ConvertId** операции веб-служб Exchange. 
  
Операции веб-служб Exchange (EWS) **ConvertId** преобразует идентификаторы элементов и папок между форматы, поддерживаемые Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с Exchange Server 2013. 
  
## <a name="using-the-convertid-operation"></a>С помощью операции ConvertId
<a name="bk_usingConvertId"> </a>

Следующие идентификаторы можно преобразовать с помощью операции **ConvertId** : 
  
- Формат идентификатора для веб-служб Exchange в первоначальной версии Exchange 2007. Представляет `EwsLegacyId` значение перечисления в перечислении [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- Формат идентификатора для веб-служб Exchange в Exchange 2007 с пакетом обновления 1 или Exchange 2010. Представляет `EwsId` значение перечисления в [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Идентификатор MAPI, как и свойство **PR_ENTRYID** . Представляет `EntryId` значение перечисления в перечислении [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- Идентификатор события календаря доступности. Это представление шестнадцатеричном формате **PR_ENTRYID** свойства. Представляет `HexEntryId` значение перечисления в [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Идентификатор хранилища Exchange. Представляет `StoreId` значение перечисления в [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). Операция **ConvertId** не преобразует идентификаторы общедоступных папок из идентификатора веб-служб Exchange на идентификатор хранилища. 
    
- Идентификатор Outlook Web App. Представляет `OwaId` значение перечисления в [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Передача URL-адреса, создаваемые из этот идентификатор в Outlook Web App не поддерживается. Идентификатор Outlook Web App можно применять к Exchange 2007 и Exchange 2010. Outlook Web App для Exchange Online и версии Exchange, начиная с Exchange Server 2013 использует идентификаторы веб-служб Exchange.
    
Операция **ConvertId** работать неправильно при преобразовании идентификаторы общедоступных папок из идентификатора веб-служб Exchange с идентификатором хранилища в Exchange Online и Exchange 2013. Идентификатор, который возвращается в качестве решения можно обновлять вручную. Чтобы вручную обновить идентификатор: 
  
1. В коде приложения определите, является ли элемент или папку в общей папке. 
    
2. Декодирования строка идентификатора кодировке Base64.
    
3. Убедитесь, что тип byte (21 байтов) имеет значение 7. Значение 7 указывает, что идентификатор является неверный формат.
    
4. Пропустите первые четыре байта. Они должны иметь значение нулю.
    
5. Обновление следующего 16 байт с помощью следующих GUID: 1A447390AA6611CD9BC800AA002FC45A
    
6. Обновите следующий байт (типа byte) со значением 9.
    
7. Измените идентификатор строка в кодировке Base64.
    
> [!NOTE]
> Операция **ConvertId** проверяет, что для данного SMTP-адрес имеет допустимый формат. Операция не определяет, представляет ли SMTP-адрес допустимым почтового ящика. 
  
Операция **ConvertId** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
**В таблице 1. Заголовки SOAP ConvertId операции**

|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Это применимо к запросу.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции, которые применяются к запросу.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Это применимо для ответа.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Пример запроса ConvertId операции
<a name="bk_usingConvertId"> </a>

В следующем примере запрос **ConvertId** показано, как для преобразования из идентификатора веб-служб Exchange в Outlook Web App идентификатора. 
  
Необходимо задать элемент [RequestServerVersion](requestserverversion.md) в заголовке SOAP, чтобы Exchange2007_SP1 или более поздней версии для успешного выполнения этой операции. 
  
> [!NOTE]
> Идентификатор элемента был усечен, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>Пример ответа ConvertId операции
<a name="bk_usingConvertId"> </a>

В следующем примере показано успешного ответа на запрос **ConvertId** . В этом примере ответа содержит идентификатор Outlook Web App. 
  
> [!NOTE]
> Идентификатор Outlook Web App был усечен, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <AlternateId xsi:type="t:AlternateIdType" Format="OwaId" Id="RgAAAAAS2%2" 
                         Mailbox="user@example.com" />
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-error-response-example"></a>Пример ответа об ошибке ConvertId операции
<a name="bk_usingConvertId"> </a>

В следующем примере показано ответа на запрос, который содержит неверный тип формат идентификатора.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Error">
          <MessageText>Id is malformed.</MessageText>
          <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
          <DescriptiveLinkKey>0</DescriptiveLinkKey>
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="version-differences"></a>Различия версий
<a name="bk_ConvertIdVersionDiff"> </a>

Формат идентификатора веб-служб Exchange, изменились при переходе от первоначальной версии Exchange 2007 и Exchange 2007 с пакетом обновления 1 (SP1). Exchange Online в составе Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2010 использовать тот же идентификатор формат, который использует Exchange 2007 с пакетом обновления 1.
  
Операция **ConvertId** преобразует идентификаторы общедоступных папок из идентификатора веб-служб Exchange идентификатор хранилища в Exchange 2007 и Exchange 2010. 
  
## <a name="see-also"></a>См. также
<a name="bk_ConvertIdVersionDiff"> </a>

- [Преобразование идентификаторов](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

