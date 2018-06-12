---
title: Операция GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Найдите сведения о веб-служб Exchange GetSearchableMailboxes операции.
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762910"
---
# <a name="getsearchablemailboxes-operation"></a>Операция GetSearchableMailboxes

Найдите сведения о **GetSearchableMailboxes** операции веб-служб Exchange. 
  
Операция **GetSearchableMailboxes** получает областью видимости набора для поиска почтовых ящиков для операций поиска обнаружения. Область поиска почтовых ящиков, возвращаемого в ответе определяется поисковый фильтр и ли расширенное членство в группах рассылки. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getsearchablemailboxes-operation"></a>С помощью операции GetSearchableMailboxes

Операция **GetSearchableMailboxes** получает сведения о почтовых ящиках с возможностью поиска. Следующие аргументы могут передаваться в запросе: 
  
- [SearchFilter](searchfilter.md) — принимает псевдоним одного адреса электронной почты в качестве аргумента. 
    
- [ExpandGroupMembership](expandgroupmembership.md) — указывает, развернут ли группы рассылки в списке результатов, возвращаемого в ответе. 
    
Если группа рассылки — это псевдоним электронной почты, задайте в фильтре поиска и членство в группах рассылки не развернут, ответ будет содержать сведения о почтовых ящиках для группы рассылки. Если группа рассылки — это псевдоним электронной почты, задайте в поисковый фильтр и расширенное членство в группах рассылки, ответ будет содержать сведения о почтовых ящиках для каждого почтового ящика, который является членом группы рассылки. Если фильтр поиска содержит псевдоним одного пользователя, ответ будет содержать сведения о почтовых ящиках для одного пользователя. Ответ будет содержать все почтовые ящики с возможностью поиска, если элемент [GetSearchableMailboxes](getsearchablemailboxes.md) пуст. Это то же, как имеющий пустой элемент [SearchFilter](searchfilter.md) и [ExpandGroupMembership](expandgroupmembership.md) элемент, значение **false**.
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a>Заголовки SOAP GetSearchableMailboxes операции

Операция **GetSearchableMailboxes** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Идентифицирует ролей сервера, необходимых в порядке для абонентов для запроса. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a>Пример запроса операции GetSearchableMailboxes: запрос сведений о группе рассылки

В следующем примере запрос операции **GetSearchableMailboxes** показано, как получить сведения о почтовых ящиках для группы рассылки lolgroup. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Запрос SOAP body содержит следующие элементы:
  
- [GetSearchableMailboxes](getsearchablemailboxes.md)
    
- [SearchFilter](searchfilter.md)
    
- [ExpandGroupMembership](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a>Успешные операции ответа GetSearchableMailboxes: получение сведений о группе рассылки

В следующем примере показано успешного ответа на запрос операции **GetSearchableMailboxes** для получения сведений обнаружения lolgroup группу рассылки. 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

Ответ SOAP body содержит следующие элементы:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [Guid](guid-ex15websvcsotherref.md)
    
- [Параметр PrimarySmtpAddress](primarysmtpaddress.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ReferenceId](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a>Успешные операции ответа GetSearchableMailboxes: получение сведений о расширенной группы рассылки

В следующем примере показано успешного ответа на запрос операции **GetSearchableMailboxes** для получения обнаружения сведений о членов группы рассылки расширенное lolgroup. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

Ответ SOAP body содержит следующие элементы:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [Guid](guid-ex15websvcsotherref.md)
    
- [Параметр PrimarySmtpAddress](primarysmtpaddress.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ReferenceId](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a>Ошибка операции GetSearchableMailboxes ответа

В следующем примере показано ошибочный ответ на запрос операции **GetSearchableMailboxes** . Это ответ на запрос для получения всех почтовых ящиков с возможностью поиска, если аргумент **ExpandGroupMembership** имеет значение **true**. 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Ошибка ответ SOAP body содержит следующие элементы:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Операция SearchMailboxes](searchmailboxes-operation.md)
    
- [Операция GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

