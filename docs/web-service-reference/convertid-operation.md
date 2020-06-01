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
description: Поиск сведений о ConvertIdной операции EWS.
ms.openlocfilehash: 36bd47d3fc7c7ca7cea7b38222abb25fba6074ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452554"
---
# <a name="convertid-operation"></a>Операция ConvertId

Поиск сведений о **ConvertIdной** операции EWS. 
  
**ConvertId** веб-служб Exchange (EWS) преобразует идентификаторы элементов и папок между форматами, принятыми Exchange Online, Exchange Online в составе Office 365, и локальными версиями Exchange, начиная с Exchange Server 2013. 
  
## <a name="using-the-convertid-operation"></a>Использование операции ConvertId
<a name="bk_usingConvertId"> </a>

С помощью операции **ConvertId** можно преобразовать следующие идентификаторы: 
  
- Формат идентификатора для EWS в первой версии Exchange 2007. Представляется `EwsLegacyId` значением перечисления в перечислении [идформат](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- Формат идентификатора для EWS в Exchange 2007 с пакетом обновления 1 (SP1) или Exchange 2010. Представляется `EwsId` значением перечисления в [идформат](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Идентификатор MAPI, как в свойстве **PR_ENTRYID** . Представляется `EntryId` значением перечисления в перечислении [идформат](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- Идентификатор события календаря доступности. Это представление свойства **PR_ENTRYID** в шестнадцатеричной кодировке. Представляется `HexEntryId` значением перечисления в [идформат](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- Идентификатор хранилища Exchange. Представляется `StoreId` значением перечисления в [идформат](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). Операция **ConvertId** не преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор хранилища. 
    
- Идентификатор Outlook Web App. Представляется `OwaId` значением перечисления в [идформат](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Передача URL-адресов, созданных из этого идентификатора в Outlook Web App, не поддерживается. Идентификатор Outlook Web App применяется к Exchange 2007 и Exchange 2010. Outlook Web App для Exchange Online и версии Exchange, начиная с Exchange Server 2013, используют идентификаторы EWS.
    
Операция **ConvertId** не работает должным образом при преобразовании идентификаторов общедоступных папок из идентификатора EWS в идентификатор хранилища в Exchange Online и Exchange 2013. Вы можете вручную обновить идентификатор, возвращаемый в качестве обходного пути. Чтобы вручную обновить идентификатор, выполните следующие действия: 
  
1. В коде приложения определите, находится ли целевой элемент или папка в общедоступной папке. 
    
2. Расшифровать строку идентификатора в кодировке Base64.
    
3. Убедитесь, что тип Byte (21-байтовый) имеет значение 7. Значение 7 указывает на то, что идентификатор имеет недопустимый формат.
    
4. Пропустите первые четыре байта. Им необходимо присвоить нулевое значение.
    
5. Обновите следующие 16 байт с помощью следующего GUID: 1A447390AA6611CD9BC800AA002FC45A
    
6. Обновите следующий байт (тип Byte) со значением 9.
    
7. Замените идентификатор на строку в кодировке Base64.
    
> [!NOTE]
> Операция **ConvertId** проверяет, что заданный SMTP-адрес имеет допустимый формат. Эта операция не определяет, представляет ли SMTP-адрес действительный почтовый ящик. 
  
Операция **ConvertId** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
**Таблица 1. Заголовки SOAP операции ConvertId**

|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Это относится к запросу.  <br/> |
|рекуестверсион  <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции это относится к запросу.  <br/> |
|серверверсион  <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Это относится к отклику.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Пример запроса операции ConvertId
<a name="bk_usingConvertId"> </a>

В приведенном ниже примере запроса **ConvertId** показано, как преобразовать идентификатор EWS в идентификатор Outlook Web App. 
  
Чтобы эта операция работала, элемент [рекуестсерверверсион](requestserverversion.md) в заголовке SOAP должен иметь значение Exchange2007_SP1 или более поздней версии. 
  
> [!NOTE]
> Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость. 
  
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

## <a name="convertid-operation-response-example"></a>Пример ответа операции ConvertId
<a name="bk_usingConvertId"> </a>

В следующем примере показан успешный ответ на запрос **ConvertId** . В этом примере ответа содержится идентификатор Outlook Web App. 
  
> [!NOTE]
> Идентификатор Outlook Web App был сокращен, чтобы сохранить удобочитаемость. 
  
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

## <a name="convertid-operation-error-response-example"></a>Пример ответа на сообщение об ошибке операции ConvertId
<a name="bk_usingConvertId"> </a>

В следующем примере показан ответ на запрос, который содержит недопустимый тип формата идентификатора.
  
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

Формат идентификатора EWS изменился между исходной версией Exchange 2007 и Exchange 2007 с пакетом обновления 1 (SP1). Exchange Online в составе Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2010, используют тот же формат идентификатора, который использует Exchange 2007 с пакетом обновления 1 (SP1).
  
Операция **ConvertId** преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор хранилища в Exchange 2007 и Exchange 2010. 
  
## <a name="see-also"></a>См. также
<a name="bk_ConvertIdVersionDiff"> </a>

- [Преобразование идентификаторов](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [конвертидтипе](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

