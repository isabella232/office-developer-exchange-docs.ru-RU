---
title: Операция AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Поиск сведений о AddImGroupной операции EWS.
ms.openlocfilehash: 38ed12a741d46fe998dc0079ed13973ce9edf5ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462817"
---
# <a name="addimgroup-operation"></a>Операция AddImGroup

Поиск сведений о **AddImGroupной** операции EWS. 
  
При выполнении операции веб-служб Exchange **AddImGroup** в почтовый ящик добавляется новая группа обмена мгновенными сообщениями (IM). 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-addimgroup-operation"></a>Использование операции AddImGroup

Для операции **AddImGroup** используется только один аргумент Display Name. 
  
Эта операция возвращает отображаемое имя, тип группы и идентификатор хранилища Exchange для новой группы.
  
Операция **AddImGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
**Таблица 1. Заголовки SOAP операции AddImGroup**

|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Это относится к запросу.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Это относится к запросу.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Это относится к запросу.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Это относится к отклику.  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a>Пример запроса операции AddImGroup: создание новой группы для обмена мгновенными сообщениями

В следующем примере запроса операции **AddImGroup** показано, как создать группу обмена мгновенными сообщениями с именем микустомерграуп. 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

Текст SOAP Request содержит следующие элементы:
  
- [AddImGroup](addimgroup.md)
    
- [DisplayName (строка)](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a>Успешный отклик операции AddImGroup

В следующем примере показан успешный ответ на запрос операции **AddImGroup** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="349"
                           MinorBuildNumber="0"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [аддимграупреспонсе](addimgroupresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [Группа](imgroup.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ексчанжестореид](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a>Ответ об ошибке операции AddImGroup

В следующем примере показан ответ об ошибке для запроса операции **AddImGroup** . Это ответ на запрос, который содержит символ, который не может использоваться в отображаемом имени. Обратите внимание, что это неисправность SOAP, а не сообщение об ошибке на основе схемы. Отображаемое имя, отправленное в запросе, — ~! @ # $% ^ &amp; , и в &amp; символе возникает ошибка. &amp;На одиннадцатую строку и символ 33rd в полезных данных запроса. Получен ответ с кодом HTTP 500. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также

- [Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Операция RemoveImGroup](removeimgroup-operation.md)
    
- [SetImGroup](setimgroup.md)
    

