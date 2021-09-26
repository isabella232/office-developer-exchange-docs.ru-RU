---
title: Операция AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Сведения об использовании операции AddNewTelUriContactToGroup EWS.
ms.openlocfilehash: 2ad0f55c044e92e2f18a1705ab53be467a804091
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544299"
---
# <a name="addnewteluricontacttogroup-operation"></a>Операция AddNewTelUriContactToGroup

Сведения об использовании операции **AddNewTelUriContactToGroup** EWS. 
  
Операция **AddNewTelUriContactToGroup** добавляет новый контакт в группу на основе номера телефона контакта. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a>Использование операции AddNewTelUriContactToGroup

Запрос **операции AddNewTelUriContactToGroup** передает контактный телефон URI, SIP URI, номер телефона и группу, чтобы добавить контакт. Ответ **операции AddNewTelUriContactToGroup** создает персону для нового контакта. Эта операция позволяет клиентам добавлять новый контакт, даже если у контакта нет имени. 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a>Заглавные заготки операции ADDNewTelUriContactToGroup

В **операции AddNewTelUriContactToGroup** можно использовать заглавные таблицы SOAP, перечисленные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Этот заглавный заглавник применим к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру, определяемую в RFC 3066 , "Теги для идентификации языков", которая будет использоваться для доступа к почтовому ящику. Этот заглавный заглавник применим к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a>Пример запроса на операцию AddNewTelUriContactToGroup: добавление нового контакта в группу

В следующем примере запроса операции **AddNewTelUriContactToGroup** показано, как создать новый контакт и добавить новый контакт в группу обмена мгновенными сообщениями с помощью URL-адресов и SIP-адресов контакта. 
  
> [!NOTE]
> Для сохранения читаемости сокращены все идентификаторы элементов и ключи изменений в этой статье. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

Тело SOAP запроса содержит следующие элементы:
  
- [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md)
    
- [TelUriAddress](teluriaddress.md)
    
- [ImContactSipUriAddress](imcontactsipuriaddress.md)
    
- [ImTelephoneNumber](imtelephonenumber.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a>Успешный ответ операции AddNewTelUriContactToGroup

В следующем примере показан успешный ответ на запрос **операции AddNewTelUriContactToGroup** для создания контакта. Ответ содержит связанный идентификатор персоны для контакта, отображаемого имени персоны, который в данном случае основан на номере телефона контакта, и идентификатор элемента контакта, отображаемого в рамках атрибуции исходных идентификаторов. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <t:PersonaId Id="AAQkADE686dX3s="/>
            <t:PersonaType>Person</t:PersonaType>
            <t:CreationTime>2012-10-29T23:10:13Z</t:CreationTime>
            <t:DisplayName/>
            <t:DisplayNameFirstLast>5625550100</t:DisplayNameFirstLast>
            <t:DisplayNameLastFirst>5625550100</t:DisplayNameLastFirst>
            <t:FileAs/>
            <t:FileAsId >None</t:FileAsId>
            <t:RelevanceScore >2147483647</t:RelevanceScore>
            <t:Attributions>
               <t:Attribution>
                  <t:Id>0</t:Id>
                  <t:SourceId Id="ABhHuhCAAA=" ChangeKey="EQAAABxFU"/>
                  <t:DisplayName>Lync Contacts</t:DisplayName>
                  <t:IsWritable>false</t:IsWritable>
                  <t:IsQuickContact>true</t:IsQuickContact>
                  <t:IsHidden>false</t:IsHidden>
               </t:Attribution>
            </t:Attributions>
            <t:FileAsIds>
               <t:StringAttributedValue>
                  <t:Value>None</t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:StringAttributedValue>
            </t:FileAsIds>
            <t:OtherTelephones>
               <t:PhoneNumberAttributedValue>
                  <t:Value>
                     <t:Number>5625550100</t:Number>
                     <t:Type>Other</t:Type>
                  </t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:PhoneNumberAttributedValue>
            </t:OtherTelephones>
         </Persona>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP ответа содержит следующие элементы:
  
- [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Роль](persona.md)
    
- [PersonaId](personaid.md)
    
- [PersonaType](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [FileAsId](fileasid.md)
    
- [RelevanceScore](relevancescore.md)
    
- [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)
    
- [Attribution (PersonaAttributionType)](attribution-personaattributiontype.md)
    
- [ID (строка)](id-string.md)
    
- [SourceId](sourceid.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [IsWritable](iswritable.md)
    
- [IsQuickContact](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [FileAsIds](fileasids.md)
    
- [StringAttributedValue](stringattributedvalue.md)
    
- [Значение](value.md)
    
- [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
    
- [Attribution (строка)](attribution-string.md)
    
- [OtherTelephones](othertelephones.md)
    
- [PhoneNumberAttributedValue](phonenumberattributedvalue.md)
    
- [Значение](value.md)
    
- [Number](number.md)
    
- [Тип (строка)](type-string.md)
    
- [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
    
- [Attribution (строка)](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a>Пример ответа на ошибку при работе над операцией AddNewTelUriContactToGroup

В следующем примере показан ответ на ошибку запроса **операции AddNewTelUriContactToGroup,** когда идентификатор группы содержит хорошо сформированное значение, которое не идентифицирует группу в почтовом ящике. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP ответа на ошибку содержит следующие элементы:
  
- [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

