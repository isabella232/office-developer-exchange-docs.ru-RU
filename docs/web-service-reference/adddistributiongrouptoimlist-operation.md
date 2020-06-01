---
title: Операция AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Поиск сведений о AddDistributionGroupToImListной операции EWS.
ms.openlocfilehash: e68e21b6994af5773f5cf991d55129e1db3367ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463694"
---
# <a name="adddistributiongrouptoimlist-operation"></a>Операция AddDistributionGroupToImList

Поиск сведений о **AddDistributionGroupToImListной** операции EWS. 
  
**AddDistributionGroupToImList** веб-служб Exchange (EWS) добавляет группу рассылки в список обмена мгновенными сообщениями в едином хранилище контактов. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a>Использование операции AddDistributionGroupToImList

Операция **AddDistributionGroupToImList** принимает один аргумент, определяющий группу рассылки, которую необходимо добавить в список мгновенных сообщений. Эта операция не создает группу рассылки; Группа рассылки уже должна быть создана. 
  
Эта операция может использовать заголовки SOAP, указанные в приведенной ниже таблице.
  
**Таблица 1. Заголовки SOAP операции AddDistributionGroupToImList**

|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Это относится к запросу.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Это относится к запросу.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Это относится к запросу.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Это относится к отклику.  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a>Пример запроса операции AddDistributionGroupToImList

В следующем примере запроса операции **AddDistributionGroupToImList** показано, как добавить группу рассылки в список мгновенных сообщений. 
  
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
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

Текст SOAP Request содержит следующие элементы:
  
- [AddDistributionGroupToImList](adddistributiongrouptoimlist.md)   
- [SmtpAddress](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a>Успешный отклик операции AddDistributionGroupToImList

В следующем примере показан успешный ответ на запрос операции **AddDistributionGroupToImList** . 
  
Успешный ответ содержит отображаемое имя группы рассылки, класс хранилища Exchange для группы рассылки и идентификатор EWS новой группы рассылки.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [адддистрибутионграуптоимлистреспонсе](adddistributiongrouptoimlistresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [Группа](imgroup.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ексчанжестореид](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a>Ответ об ошибке Ерроринвалидимдистрибутионграупсмтпаддресс операции AddDistributionGroupToImList

В следующем примере показан ответ об ошибке для запроса операции **AddDistributionGroupToImList** . При попытке добавить группу рассылки, которая не существует в хранилище Exchange, возникает следующий ответ об ошибке. 
  
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
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [адддистрибутионграуптоимлистреспонсе](adddistributiongrouptoimlistresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [AddImGroup](addimgroup-operation.md)   
- [RemoveImGroup](removeimgroup-operation.md)
    

