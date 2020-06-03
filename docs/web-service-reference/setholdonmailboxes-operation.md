---
title: Операция SetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Поиск сведений о SetHoldOnMailboxesной операции EWS.
ms.openlocfilehash: 4d79ba9f616974b9415ae9eae23b8f5fdb0ab205
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448396"
---
# <a name="setholdonmailboxes-operation"></a>Операция SetHoldOnMailboxes

> [!IMPORTANT]
> Начиная с 1 апреля 2020, операция SetHoldOnMailboxes больше не будет доступна в Exchange Online. Эта операция не будет затронута в локальных версиях Exchange Server. Дополнительные сведения см. [в статье выбытие средств прежних версий электронных данных в Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).

Поиск сведений о **SetHoldOnMailboxesной** операции EWS. 
  
Операция **SetHoldOnMailboxes** задает политику хранения почтовых ящиков в почтовых ящиках. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-setholdonmailboxes-operation"></a>Использование операции SetHoldOnMailboxes

Операция **SetHoldOnMailboxes** устанавливает для почтового ящика один или несколько почтовых ящиков. 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a>Заголовки SOAP операции SetHoldOnMailboxes

Операция **SetHoldOnMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a>Пример запроса операции SetHoldOnMailboxes: применение удержания для почтового ящика

В приведенном ниже примере запроса операции **SetHoldOnMailboxes** показано, как применить удержание к двум почтовым ящикам. Удержание почтовых ящиков создано с помощью команды [New – MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SetHoldOnMailboxes>
         <m:ActionType>Create</m:ActionType>
         <m:HoldId>HoldId2</m:HoldId>
         <m:Query>test</m:Query>
         <m:Mailboxes>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</t:String>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</t:String>
         </m:Mailboxes>
         <m:Language>English</m:Language>
         <m:IncludeNonIndexableItems>false</m:IncludeNonIndexableItems>
         <m:Deduplication>true</m:Deduplication>
      </m:SetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

Текст SOAP Request содержит следующие элементы:
  
- [SetHoldOnMailboxes](setholdonmailboxes.md)
    
- [Себя (Холдактионтипе)](actiontype-holdactiontype.md)
    
- [холдид](holdid.md)
    
- [Query](query.md)
    
- [Почтовые ящики (Аррайофстрингстипе)](mailboxes-arrayofstringstype.md)
    
- [String](string.md)
    
- [Language](language.md)
    
- [инклуденониндексаблеитемс](includenonindexableitems.md)
    
- [Дедупликацию](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a>Успешный отклик операции SetHoldOnMailboxes

В следующем примере показан успешный ответ на запрос операции **SetHoldOnMailboxes** для размещения двух почтовых ящиков на удержании. 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP отклика содержит следующие элементы:
  
- [сесолдонмаилбоксесреспонсе](setholdonmailboxesresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [маилбоксхолдресулт](mailboxholdresult.md)
    
- [холдид](holdid.md)
    
- [Query](query.md)
    
- [маилбоксхолдстатусес](mailboxholdstatuses.md)
    
- [маилбоксхолдстатус](mailboxholdstatus.md)
    
- [Mailbox (строка)](mailbox-string.md)
    
- [Состояние (Холдстатустипе)](status-holdstatustype.md)
    
- [аддитионалинфо](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a>Ответ об ошибке операции SetHoldOnMailboxes

В следующем примере показан ответ об ошибке для запроса операции **SetHoldOnMailboxes** . Это ответ на запрос, который содержит неправильно указанный идентификатор почтового ящика. 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [сесолдонмаилбоксесреспонсе](setholdonmailboxesresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Операция SearchMailboxes](searchmailboxes-operation.md)
    
- [Операция GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

