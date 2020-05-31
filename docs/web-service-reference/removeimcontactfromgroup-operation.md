---
title: Операция RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: Поиск сведений о RemoveImContactFromGroupной операции EWS.
ms.openlocfilehash: 8c9af251014dbddabb439ed5bf5dc35580da6a90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835099"
---
# <a name="removeimcontactfromgroup-operation"></a>Операция RemoveImContactFromGroup

Поиск сведений о **RemoveImContactFromGroupной** операции EWS. 
  
Операция **RemoveImContactFromGroup** удаляет один контакт для обмена мгновенными сообщениями из группы обмена мгновенными сообщениями. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-removeimcontactfromgroup-operation"></a>Использование операции RemoveImContactFromGroup

Для операции **RemoveImContactFromGroup** используются два аргумента: идентификатор элемента контакта и соответствующая группа обмена мгновенными сообщениями, из которой удаляется контакт. 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a>Заголовки SOAP операции RemoveImContactFromGroup

Операция **RemoveImContactFromGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a>Пример запроса операции RemoveImContactFromGroup

В следующем примере запроса операции **RemoveImContactFromGroup** показано, как удалить контакт для обмена мгновенными сообщениями из группы обмена мгновенными сообщениями. 
  
> [!NOTE]
> Идентификаторы групп и контактов были сокращены, чтобы сохранить удобочитаемость. 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

Текст SOAP Request содержит следующие элементы:
  
- [RemoveImContactFromGroup](removeimcontactfromgroup.md)
    
- [ContactId](contactid.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a>Успешный отклик операции RemoveImContactFromGroup

В следующем примере показан успешный ответ на запрос операции **RemoveImContactFromGroup** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [ремовеимконтактфромграупреспонсе](removeimcontactfromgroupresponse.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a>Ответ об ошибке Ерроринвалидимконтактид операции RemoveImContactFromGroup

В следующем примере показан ответ об ошибке для запроса операции **RemoveImContactFromGroup** . При попытке удалить элемент контакта, который не существует в группе IM, возникает следующий ответ об ошибке. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [ремовеимконтактфромграупреспонсе](removeimcontactfromgroupresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Пользователи и контакты в EWS для Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md)
    
- [AddImContactToGroup](addimcontacttogroup-operation.md)
    
- [Операция AddImGroup](addimgroup-operation.md)
    
- [Операция AddNewImContactToGroup](addnewimcontacttogroup-operation.md)
    
- [Операция GetImItemList](getimitemlist-operation.md)
    
- [GetImItems](getimitems-operation.md)
    
- [RemoveContactFromImList](removecontactfromimlist-operation.md)
    
- [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist-operation.md)
    
- [Операция RemoveImGroup](removeimgroup-operation.md)
    
- [Операция SetImGroup](setimgroup-operation.md)
    
- [сетимлистмигратионкомплетед](setimlistmigrationcompleted-operation.md)
    

