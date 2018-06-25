---
title: Операция FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Найдите сведения о веб-служб Exchange FindPeople операции.
ms.openlocfilehash: 97c34d7df590d20513e8f1ad476d62f16815a42b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762590"
---
# <a name="findpeople-operation"></a>Операция FindPeople

Найдите сведения о **FindPeople** операции веб-служб Exchange. 
  
Операция **FindPeople** возвращает все объекты пользователя из указанной папки контактов или получает контакты, соответствующие указанному запросу строки. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-findpeople-operation"></a>С помощью операции FindPeople

Операция **FindPeople** возвращает объединенные контактные сведения. 
  
Операция **FindPeople** построена на существующую функциональность [ограничение](restriction.md) и [BaseShape](baseshape.md) сложные типы, добавив ограничение объединение и возможность получить дополнительные свойства. С помощью ограничения клиента можно указать фильтры, такие как «возвращать только результаты с адресом обмена мгновенными Сообщениями». Параметры поиска по умолчанию предназначен для указанного пользователя личных почтовых ящиков и глобальный список адресов (GAL). При поиске в глобальном списке адресов как папки поиска, необходимо указать строку запроса вместо ограничение, поскольку эта операция не позволяет для просмотра глобального списка адресов. 
  
### <a name="findpeople-operation-soap-headers"></a>Заголовки SOAP FindPeople операции

Операция **FindPeople** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="findpeople-operation-request-example"></a>Пример запроса FindPeople операции

В следующем примере запрос операции **FindPeople** показано, как возвратить первые 100 контакты из папки «Контакты». 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:FindPeople>
         <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="contacts"/>
         </m:ParentFolderId>
      </m:FindPeople>
   </soap:Body>
</soap:Envelope>
```

Запрос SOAP body содержит следующие элементы:
  
- [FindPeople](findpeople.md)
    
- [IndexedPageItemView](indexedpageitemview.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
В следующем примере запрос операции **FindPeople** показано, как возвратить первые 100 контактов из глобального списка адресов с помощью строки запроса. Установка **DistinguishedFolderId** «каталог» выполняет поиск глобального списка адресов как основной источник пользователей. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
    <m:FindPeople>
      <m:PersonaShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="persona:DisplayName"/>
          <t:FieldURI FieldURI="persona:Title"/>
        </t:AdditionalProperties>
      </m:PersonaShape>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="directory"/>
      </m:ParentFolderId>
      <m:QueryString>adams</m:QueryString>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-findpeople-operation-response"></a>Успешные операции ответа FindPeople

В следующем примере показано успешного ответа на запрос операции **FindPeople** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAOjFqObcLmtOlzlRnHdXQjo=" />
          <CreationTime>2012-01-11T22:25:37Z</CreationTime>
          <DisplayName>Terry Adams</DisplayName>
          <DisplayNameFirstLast>Terry Adams</DisplayNameFirstLast>
          <DisplayNameLastFirst>Adams Terry</DisplayNameLastFirst>
          <FileAs>Adams, Terry</FileAs>
          <GivenName>Terry</GivenName>
          <Surname>Adams</Surname>
          <EmailAddress>
            <Name>terry@litwareinc.com</Name>
            <EmailAddress>terry@litwareinc.com</EmailAddress>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
          <EmailAddresses>
            <EmailAddress>
              <Name>terry@litwareinc.com</Name>
              <EmailAddress>terry@litwareinc.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
            <EmailAddress>
              <Name>tadams@contoso.com</Name>
              <EmailAddress>tadams@contoso.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
          </EmailAddresses>
          <RelevanceScore>2147483647</RelevanceScore>
        </Persona>
      </People>
      <TotalNumberOfPeopleInView>1</TotalNumberOfPeopleInView>
    </FindPeopleResponse>
  </s:Body>
</s:Envelope>
```

Ответ SOAP body содержит следующие элементы:
  
- [FindPeopleResponse](findpeopleresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Людей](people.md)
    
- [Пользователь](persona.md)
    
- [PersonaId](personaid.md)
    
- [CreationTime](creationtime.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [GivenName](givenname.md)
    
- [Фамилия](surname.md)
    
- [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md)
    
- [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [RelevanceScore](relevancescore.md)
    
- [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a>Ошибка операции FindPeople ответа

Коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Пользователи и контакты в EWS для Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Операция GetPersona](getpersona-operation.md)
    

