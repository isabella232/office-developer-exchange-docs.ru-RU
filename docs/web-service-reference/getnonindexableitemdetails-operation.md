---
title: Операция GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: Поиск сведений о GetNonIndexableItemDetailsной операции EWS.
ms.openlocfilehash: a443e04b0622ddbaaeb1bc8c04bfd05679c6207e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530213"
---
# <a name="getnonindexableitemdetails-operation"></a>Операция GetNonIndexableItemDetails

Поиск сведений о **GetNonIndexableItemDetailsной** операции EWS. 
  
Операция **GetNonIndexableItemDetails** получает сведения об элементах, которые не удается индексировать. Это относится только к идентификатору элемента, к коду ошибки, описанию ошибки, при попытке индексирования элемента и дополнительной информации о файле. 
  
> [!NOTE]
> Несмотря на то что схема указывает на то, что можно выполнять поиск в нескольких почтовых ящиках, в исходной версии Exchange 2013 служба поддерживает только извлечение сведений об элементах для неиндексируемых элементов в одном почтовом ящике. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getnonindexableitemdetails-operation"></a>Использование операции GetNonIndexableItemDetails

Операция **GetNonIndexableItemDetails** определяет элементы почтового ящика, которые не удается индексировать, и предоставляет сведения о причинах, по которым не удается индексировать элементы. Элементы, которые не могут индексироваться, не ищутся во время поиска обнаружения. 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a>Заголовки SOAP операции GetNonIndexableItemDetails

Операция **GetNonIndexableItemDetails** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a>Пример запроса операции GetNonIndexableItemDetails: получение сведений о элементе, который не удается индексировать

В приведенном ниже примере запроса операции **GetNonIndexableItemDetails** показано, как запросить сведения для элементов, которые не удается индексировать для одного почтового ящика. Поиск выполняется как в основном, так и в архивных почтовых ящиках. 
  
> [!NOTE]
> Все устаревшие доменные имена в этом примере сокращены, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Текст SOAP Request содержит следующие элементы:
  
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [Почтовые ящики (Нонемптяррайофлегациднстипе)](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [LegacyDN](legacydn.md)
    
- [сеарчарчивеонли](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a>Успешный отклик операции GetNonIndexableItemDetails

В следующем примере показан успешный ответ на запрос операции **GetNonIndexableItemDetails** для получения элементов, которые не удается индексировать для одного почтового ящика. В этом примере элемент, который не удается индексировать, — это файл бинарифиле. ABC, который имеет неизвестный формат. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Тело SOAP отклика содержит следующие элементы:
  
- [жетнониндексаблеитемдетаилсреспонсе](getnonindexableitemdetailsresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [нониндексаблеитемдетаилсресулт](nonindexableitemdetailsresult.md)
    
- [нониндексаблеитемдетаил](nonindexableitemdetail.md)
    
- [Идентификатор](itemid.md)
    
- [ErrorCode (Итеминдексеррортипе)](errorcode-itemindexerrortype.md)
    
- [еррордескриптион](errordescription.md)
    
- [испартиаллиндексед](ispartiallyindexed.md)
    
- [исперманентфаилуре](ispermanentfailure.md)
    
- [сортвалуе](sortvalue.md)
    
- [аттемпткаунт](attemptcount.md)
    
- [ластаттемпттиме](lastattempttime.md)
    
- [аддитионалинфо](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a>Ответ об ошибке операции GetNonIndexableItemDetails

В следующем примере показан ответ об ошибке для запроса операции **GetNonIndexableItemDetails** . Это ответ на запрос получения сведений об элементах, которые не удается индексировать из нескольких почтовых ящиков. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [жетнониндексаблеитемдетаилсреспонсе](getnonindexableitemdetailsresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Операция SearchMailboxes](searchmailboxes-operation.md)
    
- [Операция GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Операция SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

