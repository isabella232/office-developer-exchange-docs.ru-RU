---
title: Операция GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: Найдите сведения о веб-служб Exchange GetNonIndexableItemDetails операции.
ms.openlocfilehash: 6b0c5afd54ac98f89bc6c5199300c20862c6f207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762857"
---
# <a name="getnonindexableitemdetails-operation"></a>Операция GetNonIndexableItemDetails

Найдите сведения о **GetNonIndexableItemDetails** операции веб-служб Exchange. 
  
Операция **GetNonIndexableItemDetails** извлекаются сведения об элементах, которые не могут быть индексированы. Это включает в себя, но не ограничивается идентификатор элемента, код ошибки, описание ошибки при попытке индексировать элемент, а также дополнительные сведения о файле. 
  
> [!NOTE]
> Несмотря на то, что схема указывает на то, что более одного почтового ящика для поиска, в первоначальной версии Exchange 2013 служба поддерживает только получение сведений об элементе nonindexable элементов в одного почтового ящика. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getnonindexableitemdetails-operation"></a>С помощью операции GetNonIndexableItemDetails

Операция **GetNonIndexableItemDetails** определяет элементы почтовых ящиков, которые не могут быть индексированы и предоставляются сведения о почему элементы не могут быть индексированы. Во время поиска обнаружения не поиска элементов, которые не могут быть индексированы. 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a>Заголовки SOAP GetNonIndexableItemDetails операции

Операция **GetNonIndexableItemDetails** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Идентифицирует ролей сервера, необходимых в порядке для абонентов для запроса. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a>Пример запроса GetNonIndexableItemDetails операции: получение сведений элемента, не могут быть индексированы

В следующем примере запрос операции **GetNonIndexableItemDetails** показано, как для запроса сведений для элементов, которые не могут быть индексированы для одного почтового ящика. Выполняется поиск в основном и архивные почтовые ящики. 
  
> [!NOTE]
> Все устаревшие доменных имен в этом примере имеют сокращение, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

Запрос SOAP body содержит следующие элементы:
  
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [Почтовые ящики (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [LegacyDN](legacydn.md)
    
- [SearchArchiveOnly](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a>Успешные операции ответа GetNonIndexableItemDetails

В следующем примере показано успешного ответа на запрос операции **GetNonIndexableItemDetails** для получения элементов, которые не могут быть индексированы для одного почтового ящика. Элемент в этом примере, не могут быть индексированы — это файл binaryfile.abc, который имеет неизвестный формат. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

Ответ SOAP body содержит следующие элементы:
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)
    
- [NonIndexableItemDetail](nonindexableitemdetail.md)
    
- [Идентификатор элемента](itemid.md)
    
- [Код ошибки (ItemIndexErrorType)](errorcode-itemindexerrortype.md)
    
- [ErrorDescription](errordescription.md)
    
- [IsPartiallyIndexed](ispartiallyindexed.md)
    
- [IsPermanentFailure](ispermanentfailure.md)
    
- [SortValue](sortvalue.md)
    
- [AttemptCount](attemptcount.md)
    
- [LastAttemptTime](lastattempttime.md)
    
- [AdditionalInfo](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a>Ошибка операции GetNonIndexableItemDetails ответа

В следующем примере показано ошибочный ответ на запрос операции **GetNonIndexableItemDetails** . Это ответ на запрос для получения сведений об элементе для элементов, которые не могут быть индексированы из более одного почтового ящика. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

Ошибка ответ SOAP body содержит следующие элементы:
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Операция SearchMailboxes](searchmailboxes-operation.md)
    
- [Операция GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Операция SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

