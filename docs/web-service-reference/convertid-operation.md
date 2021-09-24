---
title: Операция ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Сведения об операции ConvertId EWS.
ms.openlocfilehash: 04f20d8446ab3117adb3f00ea17f93c068eeffb9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536633"
---
# <a name="convertid-operation"></a>Операция ConvertId

Сведения об операции **ConvertId** EWS. 
  
Операция **ConvertId** Exchange Web Services (EWS) преобразует идентификаторы элементов и папок между форматами, которые принимаются Exchange Online, Exchange Online как часть Office 365, и локальной версией Exchange начиная с Exchange Server 2013 года. 
  
## <a name="using-the-convertid-operation"></a>Использование операции ConvertId
<a name="bk_usingConvertId"> </a>

Вы можете преобразовать следующие идентификаторы с помощью операции **ConvertId:** 
  
- Формат идентификатора для EWS в начальной версии Exchange 2007 г. Это представлено `EwsLegacyId` значением переумерия в [переумериях IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- Формат идентификатора для EWS в Exchange 2007 sp1 или Exchange 2010. Это представлено  `EwsId` значением перемерения в [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Идентификатор MAPI, как и **в PR_ENTRYID** свойстве. Это представлено `EntryId` значением переумерия в [переумериях IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- Идентификатор событий календаря доступности. Это кодированное с гексадецимальным кодом представление свойства **PR_ENTRYID.** Это представлено  `HexEntryId` значением перемерения в [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Идентификатор Exchange магазина. Это представлено  `StoreId` значением перемерения в [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). Операция **ConvertId** не преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор магазина. 
    
- Идентификатор Outlook Web App. Это представлено  `OwaId` значением переоформления [в IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Передача URL-адресов, созданных из этого идентификатора в Outlook Web App не поддерживается. Идентификатор Outlook Web App применим к Exchange 2007 и Exchange 2010. Outlook Web App для Exchange Online и версий Exchange начиная с 2013 Exchange Server использует идентификаторы EWS.
    
Операция **ConvertId** работает не так, как ожидалось, при преобразовании идентификаторов общедоступных папок из идентификатора EWS в идентификатор магазина в Exchange Online и Exchange 2013 г. Вы можете вручную обновить идентификатор, возвращаемый в качестве обходного решения. Чтобы вручную обновить идентификатор: 
  
1. В коде приложения определите, находится ли целевой элемент или папка в общедоступных папках. 
    
2. Расшифровка строки идентификатора с кодом Base64.
    
3. Убедитесь, что тип byte (21st byte) имеет значение 7. Значение 7 указывает, что идентификатор находится в неправильном формате.
    
4. Пропустить первые четыре bytes. Их необходимо установить до нуля.
    
5. Обновление следующих 16 bytes с помощью следующего GUID: 1A447390AA66611CD9BC800AA002FC45A
    
6. Обновление следующего byte (тип byte) со значением 9.
    
7. Измените идентификатор на строку с кодом Base64.
    
> [!NOTE]
> Операция **ConvertId** проверяет, что данный SMTP-адрес имеет допустимый формат. Операция не определяет, представляет ли SMTP-адрес допустимый почтовый ящик. 
  
В **операции ConvertId** можно использовать заглавные таблицы SOAP, указанные в следующей таблице. 
  
**Таблица 1. Заготчики операции ConvertId**

|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Это применимо к запросу.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции Это применимо к запросу.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Это применимо к ответу.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Пример запроса на операцию ConvertId
<a name="bk_usingConvertId"> </a>

В следующем примере **запроса ConvertId** показано, как преобразовать из идентификатора EWS в идентификатор Outlook Web App. 
  
Элемент [RequestServerVersion](requestserverversion.md) в загонах SOAP должен быть Exchange2007_SP1 или более поздней версии для работы этой операции. 
  
> [!NOTE]
> Идентификатор элемента был сокращен для сохранения читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>Пример ответа на операции ConvertId
<a name="bk_usingConvertId"> </a>

В следующем примере показан успешный ответ на запрос **ConvertId.** В этом примере ответа Outlook Web App идентификатор. 
  
> [!NOTE]
> Идентификатор Outlook Web App был сокращен для сохранения читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="convertid-operation-error-response-example"></a>Пример ответа на ошибку операции ConvertId
<a name="bk_usingConvertId"> </a>

В следующем примере показан ответ на запрос, содержащий неправильный тип формата идентификатора.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Формат идентификатора EWS изменился между начальной версией выпуска Exchange 2007 и Exchange 2007 Пакет обновления 1 (SP1). Exchange Online в Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2010 г., используют тот же формат идентификатора, что и Exchange 2007 г. sp1.
  
Операция **ConvertId** преобразует идентификаторы общедоступных папок из идентификатора EW Exchange S в идентификатор магазина в 2007 и Exchange 2010 г. 
  
## <a name="see-also"></a>См. также
<a name="bk_ConvertIdVersionDiff"> </a>

- [Преобразование идентификаторов](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

