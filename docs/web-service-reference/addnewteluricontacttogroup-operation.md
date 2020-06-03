---
title: Операция AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Найдите сведения об использовании операции AddNewTelUriContactToGroup EWS.
ms.openlocfilehash: 91228ec627ad928d2f1837c135af24846f811b1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464947"
---
# <a name="addnewteluricontacttogroup-operation"></a>Операция AddNewTelUriContactToGroup

Найдите сведения об использовании операции **AddNewTelUriContactToGroup** EWS. 
  
Операция **AddNewTelUriContactToGroup** добавляет новый контакт в группу на основе номера телефона контакта. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a>Использование операции AddNewTelUriContactToGroup

Запрос операции **AddNewTelUriContactToGroup** передает URI TEL контакта, универсальный код ресурса (URI) SIP, номер телефона и группу, в которую добавляется контакт. Ответ операции **AddNewTelUriContactToGroup** создает пользователя для нового контакта. Эта операция позволяет клиентам добавлять новый контакт, даже если у него нет имени. 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a>Заголовки SOAP операции AddNewTelUriContactToGroup

Операция **AddNewTelUriContactToGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a>Пример запроса операции AddNewTelUriContactToGroup: Добавление нового контакта в группу

В следующем примере запроса операции **AddNewTelUriContactToGroup** показано, как создать новый контакт и добавить новый контакт в группу обмена мгновенными сообщениями с помощью URI TEL и SIP контакта. 
  
> [!NOTE]
> Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость. 
  
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

Текст SOAP Request содержит следующие элементы:
  
- [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md)
    
- [телуриаддресс](teluriaddress.md)
    
- [имконтактсипуриаддресс](imcontactsipuriaddress.md)
    
- [имтелефоненумбер](imtelephonenumber.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a>Успешный отклик операции AddNewTelUriContactToGroup

В следующем примере показан успешный ответ на запрос операции **AddNewTelUriContactToGroup** для создания контакта. Ответ содержит связанный идентификатор персонажа для контакта, отображаемое имя пользователя, которое в данном случае основано на номере телефона контакта, и идентификатор элемента контакта, который отображается как часть атрибутов идентификатора источника. 
  
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

Тело SOAP отклика содержит следующие элементы:
  
- [аддневтелуриконтакттограупреспонсе](addnewteluricontacttogroupresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [Роль](persona.md)
    
- [персонаид](personaid.md)
    
- [персонатипе](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [дисплайнамефирстласт](displaynamefirstlast.md)
    
- [дисплайнамеластфирст](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [филеасид](fileasid.md)
    
- [релеванцескоре](relevancescore.md)
    
- [Атрибуты (Аррайофперсонааттрибутионстипе)](attributions-arrayofpersonaattributionstype.md)
    
- [Атрибуты (Персонааттрибутионтипе)](attribution-personaattributiontype.md)
    
- [ID (строка)](id-string.md)
    
- [SourceId](sourceid.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [Доступный для записи](iswritable.md)
    
- [искуиккконтакт](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [филеасидс](fileasids.md)
    
- [стрингаттрибутедвалуе](stringattributedvalue.md)
    
- [Значение](value.md)
    
- [Атрибуты (Аррайофвалуеаттрибутионстипе)](attributions-arrayofvalueattributionstype.md)
    
- [Атрибуты (строка)](attribution-string.md)
    
- [осертелефонес](othertelephones.md)
    
- [фоненумбераттрибутедвалуе](phonenumberattributedvalue.md)
    
- [Значение](value.md)
    
- [Number](number.md)
    
- [Тип (строка)](type-string.md)
    
- [Атрибуты (Аррайофвалуеаттрибутионстипе)](attributions-arrayofvalueattributionstype.md)
    
- [Атрибуты (строка)](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a>Пример ответа на сообщение об ошибке операции AddNewTelUriContactToGroup

В следующем примере показан ответ об ошибке для запроса операции **AddNewTelUriContactToGroup** , когда идентификатор группы содержит правильное значение, не идентифицирующее группу в почтовом ящике. 
  
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

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [аддневтелуриконтакттограупреспонсе](addnewteluricontacttogroupresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

