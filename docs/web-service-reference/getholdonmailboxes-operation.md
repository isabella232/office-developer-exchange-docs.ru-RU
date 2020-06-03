---
title: Операция GetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Поиск сведений о GetHoldOnMailboxesной операции EWS.
ms.openlocfilehash: 867f38be87e60af8708eeb0b9d0e3ac8eee6ff64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457734"
---
# <a name="getholdonmailboxes-operation"></a>Операция GetHoldOnMailboxes

> [!IMPORTANT]
> Начиная с 1 апреля 2020, операция GetHoldOnMailboxes больше не будет доступна в Exchange Online. Эта операция не будет затронута в локальных версиях Exchange Server. Дополнительные сведения см. [в статье выбытие средств прежних версий электронных данных в Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).

Поиск сведений о **GetHoldOnMailboxesной** операции EWS. 
  
Операция **GetHoldOnMailboxes** получает почтовые ящики, которые находятся в определенном удержании и связанном запросе удержания. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getholdonmailboxes-operation"></a>Использование операции GetHoldOnMailboxes

Операция **GetHoldOnMailboxes** предоставляет клиенту сведения о том, какие почтовые ящики помещаются в конкретное удержание, сведения о запросе удержания, связанном с каждым удержанием, если это необходимо, и сведения о состоянии удержания для каждого почтового ящика. Дополнительные сведения о удержаниях почтовых ящиков, в том числе о удержаниях на основе запросов, можно найти [в статье удержание на месте](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) на сайте TechNet. 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a>Заголовки SOAP операции GetHoldOnMailboxes

Операция **GetHoldOnMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a>Пример запроса операции GetHoldOnMailboxes: получение сведений о удержании почтовых ящиков

В следующем примере запроса операции **GetHoldOnMailboxes** показано, как получить сведения о удержании почтовых ящиков для хранения почтовых ящиков HoldId2. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetHoldOnMailboxes>
         <m:HoldId>HoldId2</m:HoldId>
      </m:GetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

Текст SOAP Request содержит следующие элементы:
  
- [GetHoldOnMailboxes](getholdonmailboxes.md)
    
- [холдид](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a>Успешный отклик операции GetHoldOnMailboxes

В следующем примере показан успешный ответ на запрос операции **GetHoldOnMailboxes** для получения сведений о удержании почтовых ящиков для хранения почтовых ящиков HoldId2. 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=ecc0fd98c2cadf-Willi</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=dasdat341q8de95-Micha</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP отклика содержит следующие элементы:
  
- [жесолдонмаилбоксесреспонсе](getholdonmailboxesresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [маилбоксхолдресулт](mailboxholdresult.md)
    
- [холдид](holdid.md)
    
- [Query](query.md)
    
- [маилбоксхолдстатусес](mailboxholdstatuses.md)
    
- [маилбоксхолдстатус](mailboxholdstatus.md)
    
- [Mailbox (строка)](mailbox-string.md)
    
- [Состояние (Холдстатустипе)](status-holdstatustype.md)
    
- [аддитионалинфо](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a>Ответ об ошибке операции GetHoldOnMailboxes

В следующем примере показан ответ об ошибке для запроса операции **GetHoldOnMailboxes** . Это ответ на запрос на получение удержания, которое было удалено. 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [жесолдонмаилбоксесреспонсе](getholdonmailboxesresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Операция SearchMailboxes](searchmailboxes-operation.md)
    
- [Операция SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

