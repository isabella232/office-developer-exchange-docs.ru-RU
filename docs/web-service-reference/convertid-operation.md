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
description: Найдите сведения об операции ConvertId EWS.
ms.openlocfilehash: 36bd47d3fc7c7ca7cea7b38222abb25fba6074ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452554"
---
# <a name="convertid-operation"></a>Операция ConvertId

Найдите сведения об **операции ConvertId** EWS. 
  
Операция **ConvertId** Веб-службы Exchange (EWS) преобразует идентификаторы элементов и папок между форматами, которые принимаются Exchange Online, Exchange Online как часть Office 365, и локальной версией Exchange, начиная с Exchange Server 2013. 
  
## <a name="using-the-convertid-operation"></a>Использование операции ConvertId
<a name="bk_usingConvertId"> </a>

С помощью операции **ConvertId** можно преобразовать следующие идентификаторы: 
  
- Формат идентификатора для EWS в первоначальной версии выпуска Exchange 2007. Этот код представлен значением `EwsLegacyId` enumeration в индексе [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- Формат идентификатора для EWS в Exchange 2007 с sp1 или Exchange 2010. Это представлено значением `EwsId` нумерации в [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
- Идентификатор MAPI, как в свойстве **PR_ENTRYID.** Этот код представлен значением `EntryId` из нумерации [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- Идентификатор события календаря доступности. Это представление свойства, закодированное в **PR_ENTRYID** кодировки. Этот код представлен значением `HexEntryId` нумерации в [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
- Идентификатор магазина Exchange. Это представлено значением `StoreId` нумерации в [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) Операция **ConvertId** не преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор магазина. 
    
- Идентификатор Outlook Web App. Это представлено значением  `OwaId` нумерации в [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Передача URL-адресов, созданных из этого идентификатора в Outlook Web App не поддерживается. Идентификатор Outlook Web App применяется к Exchange 2007 и Exchange 2010. Outlook Web App Exchange Online и версии Exchange, начиная с Exchange Server 2013, используют идентификаторы EWS.
    
Операция **ConvertId** работает не так, как ожидалось при преобразовании идентификаторов общедоступных папок из идентификатора EWS в идентификатор магазина в Exchange Online и Exchange 2013. Вы можете вручную обновить идентификатор, который возвращается в качестве обходного решения. Обновление идентификатора вручную: 
  
1. В коде приложения определите, находится ли целевой элемент или папка в общедоступных папках. 
    
2. Декодировать строку идентификатора в коде Base64.
    
3. Убедитесь, что для типа "byte" (21st byte) занося значение 7. Значение 7 указывает, что идентификатор имеет неправильный формат.
    
4. Пропустите первые четыре bytes. Для них должно быть установлено значение 0.
    
5. Обновите следующие 16 bytes с помощью следующего GUID: 1A447390AA6611CD9BC800AA002FC45A
    
6. Обновите следующий (введите) значение 9.
    
7. Измените идентификатор на строку в коде Base64.
    
> [!NOTE]
> Операция **ConvertId** проверяет, имеет ли данный SMTP-адрес допустимый формат. Операция не определяет, представляет ли SMTP-адрес допустимый почтовый ящик. 
  
Операция **ConvertId** может использовать заглавные листы SOAP, перечисленные в следующей таблице. 
  
**Таблица 1. ConvertId operation SOAP headers**

|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого подает клиентский приложение. Это применимо к запросу.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Это применимо к запросу.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Это применимо к отклику.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Пример запроса на операцию ConvertId
<a name="bk_usingConvertId"> </a>

В следующем примере запроса **ConvertId** показано, как преобразовать идентификатор EWS в Outlook Web App идентификатора. 
  
Для работы этой операции необходимо установить для элемента [RequestServerVersion](requestserverversion.md) в заголе SOAP Exchange2007_SP1 или более поздней версии. 
  
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

## <a name="convertid-operation-response-example"></a>Пример отклика операции ConvertId
<a name="bk_usingConvertId"> </a>

В следующем примере показан успешный ответ на запрос **ConvertId.** В этом примере ответа содержится Outlook Web App идентификатора. 
  
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

## <a name="convertid-operation-error-response-example"></a>Пример отклика об ошибке операции ConvertId
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

Формат идентификатора EWS изменился между первоначальной версией выпуска Exchange 2007 и Exchange 2007 Пакет обновления 1 (SP1). Exchange Online в составе Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2010, использует тот же формат идентификаторов, что и Exchange 2007 с sp1.
  
Операция **ConvertId** преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор магазина в Exchange 2007 и Exchange 2010. 
  
## <a name="see-also"></a>См. также
<a name="bk_ConvertIdVersionDiff"> </a>

- [Преобразование идентификаторов](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

