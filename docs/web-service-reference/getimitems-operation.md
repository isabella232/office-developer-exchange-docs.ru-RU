---
title: Операция GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: Поиск сведений о GetImItemsной операции EWS.
ms.openlocfilehash: 4335cc22b22dc5f102f2221f7fdb22a506ba026f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762817"
---
# <a name="getimitems-operation"></a>Операция GetImItems

Поиск сведений о **GetImItemsной** операции EWS. 
  
Операция **GetImItems** получает сведения о группах обмена мгновенными сообщениями и пользователях контактов для обмена мгновенными сообщениями. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getimitems-operation"></a>Использование операции GetImItems

Операция **GetImItems** принимает идентификаторы элементов Group и Contact и возвращает набор сведений о группах и контактах. Наборы свойств, возвращаемые в ответе, идентифицируются с помощью расширенных свойств, нескольких идентификаторов контакта, идентификаторов групп и определений расширенных свойств в качестве аргументов. 
  
### <a name="getimitems-operation-soap-headers"></a>Заголовки SOAP операции GetImItems

Операция **GetImItems** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a>Пример запроса операции GetImItems: получение подробных сведений о контактах и группах для обмена мгновенными сообщениями

В следующем примере запроса операции **GetImItems** показано, как запросить подробные сведения о контактах и группах для обмена мгновенными сообщениями. Операция **GetImItems** может запросить один или несколько сведений о контакте или группе. Вы также можете использовать расширенные свойства для получения настраиваемых свойств для групп и контактов. Если запрошенное расширенное свойство не существует для элемента, то ответ будет игнорировать запрошенное свойство и возвращать ответ для набора свойств по умолчанию. В этом примере показано, как получить отображаемое имя с помощью расширенных свойств. 
  
> [!NOTE]
> Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость. Обратите внимание, что для этой операции в службе игнорируются ключи изменений. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:GetImItems>
         <m:ContactIds>
            <t:ItemId Id="AAMkADEzOTExYACABmEhpSAAA=" ChangeKey="EQAAABBmNDjF"/>
         </m:ContactIds>
         <m:GroupIds>
            <t:ItemId Id="AAMkADEzOTExYjJkBY7+0EAAA=" ChangeKey="EgAAAA=="/>
         </m:GroupIds>         
         <m:ExtendedProperties>
            <t:ExtendedProperty PropertyTag="0x3001" PropertyType="String"/>
         </m:ExtendedProperties>
      </m:GetImItems>
   </soap:Body>
</soap:Envelope>
```

Текст SOAP Request содержит следующие элементы:
  
- [GetImItems](getimitems.md)
    
- [контактидс](contactids.md)
    
- [Идентификатор](itemid.md)
    
- [граупидс](groupids.md)
    
- [Екстендедпропертиес (Нонемптяррайофекстендедфиелдурис)](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [ExtendedProperty (Пастоекстендедфиелдтипе)](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a>Успешный отклик операции GetImItems

В следующем примере показан успешный ответ на запрос **GetImItems** для получения контакта и группы для обмена мгновенными сообщениями. Отображаемое имя запрашивается в расширенном свойстве. Контакты для обмена мгновенными сообщениями возвращаются в виде пользователя. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Exchange SDK Team</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkADEzQrAABY7+0EAAA=" ChangeKey="EgAAAA=="/>
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkADEzOTExYjeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQAAAA=="/>
                  </MemberCorrelationKey>
                  <ExtendedProperties>
                     <ExtendedProperty>
                        <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                        <Value>Exchange SDK Team</Value>
                     </ExtendedProperty>
                  </ExtendedProperties>
               </ImGroup>
            </Groups>
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkADEzOTBZImBzN5J/uHXc="/>
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-11-07T00:10:35Z</CreationTime>
                  <DisplayName>Tony Smith</DisplayName>
                  <DisplayNameFirstLast>Tony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Tony Smith</DisplayNameLastFirst>
                  <FileAs/>
                  <FileAsId>None</FileAsId>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkADEzhQaoeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQArAABmNDjF"/>
                        <DisplayName>Lync Contacts</DisplayName>
                        <IsWritable>false</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
                  <ExtendedProperties>
                     <ExtendedPropertyAttributedValue>
                        <Value>
                           <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                           <Value>Tony Smith</Value>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </ExtendedPropertyAttributedValue>
                  </ExtendedProperties>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemsResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [жетимитемсреспонсе](getimitemsresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [имитемлист](imitemlist.md)
    
- [Groups (Аррайофимграуптипе)](groups-arrayofimgrouptype.md)
    
- [Группа](imgroup.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ексчанжестореид](exchangestoreid.md)
    
- [мемберкоррелатионкэй](membercorrelationkey.md)
    
- [Идентификатор](itemid.md)
    
- [Екстендедпропертиес (Нонемптяррайофекстендедфиелдурис)](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [ExtendedProperty (Пастоекстендедфиелдтипе)](extendedproperty-pathtoextendedfieldtype.md)
    
- [Фиктивные пользователи](personas-ex15websvcsotherref.md)
    
- [персонаид](personaid.md)
    
- [персонатипе](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [дисплайнамефирстласт](displaynamefirstlast.md)
    
- [дисплайнамеластфирст](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [Филеасид](fileasid.md) филеасид 
    
- [Адрес (String)](imaddress-string.md)
    
- [релеванцескоре](relevancescore.md)
    
- [Атрибуты (Аррайофперсонааттрибутионстипе)](attributions-arrayofpersonaattributionstype.md)
    
- [Атрибуты (Персонааттрибутионтипе)](attribution-personaattributiontype.md)
    
- [ID (строка)](id-string.md)
    
- [SourceId](sourceid.md)
    
- [Доступный для записи](iswritable.md)
    
- [искуиккконтакт](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [стрингаттрибутедвалуе](stringattributedvalue.md)
    
- [филеасидс](fileasids.md)
    
- [Адреса](imaddresses.md)
    
- [Значение (Екстендедпропертитипе)](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a>Ответ об ошибке операции GetImItems

Операция **GetImItems** не проверяет идентификаторы и не возвращает ожидаемый ответ об ошибке **ерроринвалидимконтактид** или **ерроринвалидимграупид** , если службе предоставлен недопустимый идентификатор контакта или группы. 
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetImItemList](getimitemlist-operation.md)
    

