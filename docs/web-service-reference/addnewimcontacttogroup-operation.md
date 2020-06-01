---
title: Операция AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Поиск сведений о AddNewImContactToGroupной операции EWS.
ms.openlocfilehash: e91cc067b4161b366e6713a9adc16873e63b1562
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465031"
---
# <a name="addnewimcontacttogroup-operation"></a>Операция AddNewImContactToGroup

Поиск сведений о **AddNewImContactToGroupной** операции EWS. 
  
Операция **AddNewImContactToGroup** добавляет новый контакт в группу мгновенных сообщений (IM). 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-addnewimcontacttogroup-operation"></a>Использование операции AddNewImContactToGroup

Для добавления нового контакта в группу обмена мгновенными сообщениями в операции **AddNewImContactToGroup** используются три указанных ниже аргумента. 
  
- Свойство " **Address** " — определяет адрес для обмена мгновенными сообщениями контакта. Это свойство является обязательным. 
    
- Свойство **DisplayName** — определяет отображаемое имя контакта. 
    
- **GroupId** свойство — определяет группу, в которую добавляется контакт. 
    
Эта операция возвращает пользователя контакта, который был добавлен в группу.
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a>Заголовки SOAP операции AddNewImContactToGroup

Операция **AddNewImContactToGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a>Пример запроса операции AddNewImContactToGroup: Добавление нового контакта для обмена мгновенными сообщениями в группу

В следующем примере запроса операции **AddNewImContactToGroup** показано, как добавить новый контакт в существующую группу обмена мгновенными сообщениями. Значение свойства **groupId** для этого примера было возвращено из результатов [операции AddImGroup](addimgroup-operation.md). Свойство **ексчанжестореид** содержит значение свойства **groupId** . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:AddNewImContactToGroup>
         <m:ImAddress>tsmith@contoso.com</m:ImAddress>
         <m:DisplayName>Tony Smith</m:DisplayName>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddNewImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> Значение **groupId** было сокращено, чтобы сохранить удобочитаемость. 
  
Текст SOAP Request содержит следующие элементы:
  
- [AddNewImContactToGroup](addnewimcontacttogroup.md)
    
- [Адрес (String)](imaddress-string.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a>Успешный отклик операции AddNewImContactToGroup

В следующем примере показан успешный ответ на запрос операции **AddNewImContactToGroup** . Ответ содержит пользователя созданного контакта. Контакт будет добавлен в папку "Быстрые контакты" в Exchange. 
  
> [!NOTE]
> Идентификаторы сокращены для сохранения удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Attribution>
            <Id>0</Id>
            <SourceId Id="BtF8oI7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                      ChangeKey="EQAAABYAAABtF8oIQoTbWAAAAAAyg" />
            <DisplayName>Outlook</DisplayName>
            <IsWritable>true</IsWritable>
            <IsQuickContact>true</IsQuickContact>
            <IsHidden>false</IsHidden>
            <FolderId Id="AAMkAGQ1MjJjMTBkLTc4YhQoTbWAAAAAAvZAAA=" 
                      ChangeKey="AQAAAA==" />
          </Attribution>
        </Attributions>
        <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddressAttributedValue>
            <Value>
              <Name>Tony Smith</Name>
              <Address>tsmith@contoso.com</Address>
              <RoutingType>SMTP</RoutingType>
            </Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </EmailAddressAttributedValue>
        </Emails1>
        <ImAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>tsmith@contoso.com</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </ImAddresses>
      </Persona>
    </AddNewImContactToGroupResponse>
  </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [аддневимконтакттограупреспонсе](addnewimcontacttogroupresponse.md)
    
- [Роль](persona.md)
    
- [персонаид](personaid.md)
    
- [персонатипе](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [дисплайнамефирстласт](displaynamefirstlast.md)
    
- [дисплайнамеластфирст](displaynamelastfirst.md)
    
- [филеасид](fileasid.md)
    
- [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [Address (строка)](address-string.md)
    
- [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [Адрес (String)](imaddress-string.md)
    
- [релеванцескоре](relevancescore.md)
    
- [Атрибуты (Аррайофперсонааттрибутионстипе)](attributions-arrayofpersonaattributionstype.md)
    
- [Атрибуты (Персонааттрибутионтипе)](attribution-personaattributiontype.md)
    
- [ID (строка)](id-string.md)
    
- [SourceId](sourceid.md)
    
- [Доступный для записи](iswritable.md)
    
- [искуиккконтакт](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [FolderId](folderid.md)
    
- [DisplayName](displaynames.md)
    
- [стрингаттрибутедвалуе](stringattributedvalue.md)
    
- [Значение (Аррайофстрингвалуетипе)](value-arrayofstringvaluetype.md)
    
- [филеасидс](fileasids.md)
    
- [Emails1](emails1.md)
    
- [емаиладдрессаттрибутедвалуе](emailaddressattributedvalue.md)
    
- [Адреса](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a>Ответ об ошибке операции AddNewImContactToGroup

В следующем примере показан ответ об ошибке для запроса операции **AddNewImContactToGroup** . Это ответ на запрос на добавление контакта в группу, которая не находится в почтовом ящике запросившего. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [аддневимконтакттограупреспонсе](addnewimcontacttogroupresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [мессажексмл](messagexml.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также



[Операция AddImGroup](addimgroup-operation.md)
  
[Операция AddImContactToGroup](addimcontacttogroup-operation.md)
  
[Операция AddImGroup](addimgroup-operation.md)
  
[Операция RemoveImGroup](removeimgroup-operation.md)
  
[Операция SetImGroup](setimgroup-operation.md)


[Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

