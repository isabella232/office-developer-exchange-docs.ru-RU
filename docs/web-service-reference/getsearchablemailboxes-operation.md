---
title: Операция GetSearchableMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Поиск сведений о GetSearchableMailboxesной операции EWS.
ms.openlocfilehash: e893a66eb1b638479eeccc6bd7548cb020f37243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530841"
---
# <a name="getsearchablemailboxes-operation"></a>Операция GetSearchableMailboxes

> [!IMPORTANT]
> Начиная с 1 апреля 2020, операция GetSearchableMailboxes больше не будет доступна в Exchange Online. Эта операция не будет затронута в локальных версиях Exchange Server. Дополнительные сведения см. [в статье выбытие средств прежних версий электронных данных в Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).

Поиск сведений о **GetSearchableMailboxesной** операции EWS. 
  
Операция **GetSearchableMailboxes** получает набор почтовых ящиков с возможностью поиска для поиска при обнаружении. Область получаемых в ответе почтовых ящиков с возможностью поиска определяется фильтром поиска и развернутой группой рассылки. 

> [!NOTE] 
> Эта операция предназначена для использования с фильтром поиска и извлечения только первых тысяч; Он не предназначен для получения исчерпывающей информации.
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getsearchablemailboxes-operation"></a>Использование операции GetSearchableMailboxes

Операция **GetSearchableMailboxes** получает сведения о почтовых ящиках с возможностью поиска. В запросе передаются следующие аргументы: 
  
- [SearchFilter](searchfilter.md) — принимает один псевдоним электронной почты в качестве аргумента. 
    
- [Експандграупмембершип](expandgroupmembership.md) — указывает, развернута ли членство в группе рассылки в результатах, возвращенных в ответе. 
    
Если набор псевдонимов электронной почты в фильтре поиска является группой рассылки, а членство в группе рассылки не развернуто, ответ будет содержать сведения о почтовом ящике для группы рассылки. Если набор псевдонимов электронной почты в фильтре поиска является группой рассылки, а членство в группе рассылки развернуто, ответ будет содержать сведения о почтовом ящике для каждого почтового ящика, который является членом группы рассылки. Если фильтр поиска содержит псевдоним одного пользователя, ответ будет содержать сведения о почтовом ящике одного пользователя. Ответ будет содержать все почтовые ящики для поиска, если элемент [GetSearchableMailboxes](getsearchablemailboxes.md) пуст. Это то же самое, что у пустого элемента [SearchFilter](searchfilter.md) , а для элемента [експандграупмембершип](expandgroupmembership.md) задано **значение false**.
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a>Заголовки SOAP операции GetSearchableMailboxes

Операция **GetSearchableMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|Имя заголовка|Элемент|Описание|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a>Пример запроса операции GetSearchableMailboxes: запрос сведений о группе рассылки

В следующем примере запроса операции **GetSearchableMailboxes** показано, как получить сведения о почтовом ящике для группы рассылки лолграуп. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetSearchableMailboxes>
         <m:SearchFilter>lolgroup</m:SearchFilter>
         <m:ExpandGroupMembership>false</m:ExpandGroupMembership>
      </m:GetSearchableMailboxes>
   </soap:Body>
</soap:Envelope>

```

Текст SOAP Request содержит следующие элементы:
  
- [GetSearchableMailboxes](getsearchablemailboxes.md)   
- [SearchFilter](searchfilter.md)    
- [експандграупмембершип](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a>Успешный отклик операции GetSearchableMailboxes: получение сведений о группе рассылки

В следующем примере показан успешный ответ на запрос операции **GetSearchableMailboxes** для получения сведений об обнаружении для группы рассылки лолграуп. 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Guid>33a408fe-2574-4e3b-49f5-5e1e000a3035</Guid>
               <PrimarySmtpAddress>LOLgroup@contoso.com</PrimarySmtpAddress>
               <IsExternalMailbox>false</IsExternalMailbox>
               <ExternalEmailAddress/>
               <DisplayName>LOLgroup</DisplayName>
               <IsMembershipGroup>true</IsMembershipGroup>
               <ReferenceId>/o=First/ou=Exchange(FYLT)/cn=Recipients/cn=81213b958a0b5295b13b3f02b812bf1bc-LOLgroup</ReferenceId>
            </SearchableMailbox>
         </SearchableMailboxes>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP отклика содержит следующие элементы:
  
- [жетсеарчаблемаилбоксесреспонсе](getsearchablemailboxesresponse.md)   
- [респонсекоде](responsecode.md)   
- [сеарчаблемаилбоксес](searchablemailboxes.md)    
- [сеарчаблемаилбокс](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [исекстерналмаилбокс](isexternalmailbox.md)   
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (строка)](displayname-string.md)    
- [исмембершипграуп](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a>Успешный отклик операции GetSearchableMailboxes: получение сведений о расширенной группе рассылки

В следующем примере показан успешный ответ на запрос операции **GetSearchableMailboxes** для получения сведений об обнаружении членов развернутой группы рассылки лолграуп. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>3c620d04-8b33-435a-95be-5b939375576</Guid>
          <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Steven Brown</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=90312341a742f0e47e392c80a60d13ecf-Steve</ReferenceId>
        </SearchableMailbox>
      </SearchableMailboxes>
    </GetSearchableMailboxesResponse>
  </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [жетсеарчаблемаилбоксесреспонсе](getsearchablemailboxesresponse.md)    
- [респонсекоде](responsecode.md)   
- [сеарчаблемаилбоксес](searchablemailboxes.md)    
- [сеарчаблемаилбокс](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [исекстерналмаилбокс](isexternalmailbox.md)    
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (строка)](displayname-string.md)    
- [исмембершипграуп](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a>Ответ об ошибке операции GetSearchableMailboxes

В следующем примере показан ответ об ошибке для запроса операции **GetSearchableMailboxes** . Это ответ на запрос на получение всех почтовых ящиков, для которых выполняется поиск, если для аргумента **експандграупмембершип** задано значение **true**. 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [жетсеарчаблемаилбоксесреспонсе](getsearchablemailboxesresponse.md)  
- [мессажетекст](messagetext.md)   
- [респонсекоде](responsecode.md)   
- [дескриптивелинккэй](descriptivelinkkey.md) 
- [сеарчаблемаилбоксес](searchablemailboxes.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)   
- [Операция SetHoldOnMailboxes](setholdonmailboxes-operation.md)   
- [Операция SearchMailboxes](searchmailboxes-operation.md)   
- [Операция GetHoldOnMailboxes](getholdonmailboxes-operation.md)    
- [Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)   
- [Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)   
- [Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

