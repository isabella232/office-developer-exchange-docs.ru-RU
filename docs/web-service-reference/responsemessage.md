---
title: ResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: Элемент ResponseMessage содержит описательные сведения о состоянии ответа для одной сущности в запросе.
ms.openlocfilehash: 69f1f6f12d10044045b72dd644536e742c479b9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835191"
---
# <a name="responsemessage"></a>ResponseMessage

Элемент **ResponseMessage** содержит описательные сведения о состоянии ответа для одной сущности в запросе. 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 **ResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Представляет состояния ответа. <br/><br/>Для этого атрибута допустимы следующие значения:  <br/><br/>-Success  <br/>-Предупреждение  <br/>-Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|Успешное выполнение  <br/> |Описание запроса, который будет выполнен.  <br/> |
|Предупреждающая  <br/> | Описание запроса, который не был обработан. Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать. <br/><br/>Ниже приведены возможные причины возникновения предупреждения.  <br/><br/>-В хранилище Exchange будут недоступны во время пакета.  <br/>-К службе каталогов Active Directory находится в автономном режиме.  <br/>-Почтовые ящики перемещаются.  <br/>-База данных сообщений (MDB) находится в автономном режиме.  <br/>-Пароль просрочен.  <br/>-Превышено квоту.  <br/> |
|Ошибка  <br/> | Описание запроса, который не может быть выполнен. <br/><br/>Ниже приведены возможные причины возникновения ошибки.  <br/><br/>-Недопустимый атрибуты и элементы  <br/>-Атрибуты или элементы вне диапазона  <br/>— Неизвестный тег  <br/>-Атрибут или элемент не допускается в контексте  <br/>— Попытка доступа не санкционировано любой клиент  <br/>-Сбой сервере в ответ на допустимый вызовов со стороны клиента  <br/> <br/> Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользуемых и зарезервирован для будущего использования. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Содержит сведения о доступности для одного почтового ящика пользователя. <br/> <br/> Ниже приведен выражение XPath 2.0 для этого элемента. <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[SuggestionsResponse](suggestionsresponse.md) <br/> |Содержит данные сведения и предложения о ответа для запроса предложений о собрании.  <br/><br/> Ниже приведен выражение XPath 2.0 для этого элемента.<br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Содержит параметры об отсутствии на работе для пользователя и результатов ответа.  <br/><br/> Ниже приведен выражение XPath 2.0 для этого элемента.  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[SetUserOofSettingsResponse](setuseroofsettingsresponse.md) <br/> |Содержит результат попытки сообщение [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) . <br/> <br/> Ниже приведен выражение XPath 2.0 для этого элемента.  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Замечания

Тип **ResponseMessageType** общими для всех ответов веб-служб Exchange. Тип **ResponseMessageType** только следующих сложных типов: 
  
- **ApplyConversationActionResponseMessageType**
    
- **AttachmentInfoResponseMessageType**
    
- **DeleteAttachmentResponseMessageType**
    
- **DeleteItemResponseMessageType**
    
- **ExpandDLResponseMessageType**
    
- **FindFolderResponseMessageType**
    
- **FindItemResponseMessageType**
    
- **FolderInfoResponseMessageType**
    
- **GetEventsResponseMessageType**
    
- **ItemInfoResponseMessageType**
    
- **ResolveNamesResponseMessageType**
    
- **SubscribeResponseMessageType**
    
- **SendNotificationResponseMessageType**
    
- **SyncFolderHierarchyResponseMessageType**
    
- **SyncFolderItemsResponseMessageType**
    
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
### <a name="version-differences"></a>Различия версий

Типы **ApplyConversationActionResponseMessage** и **DeleteItemResponseMessageType** были представлены в Exchange построения 15.00.0986.00. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)
- [Операция GetUserOofSettings](getuseroofsettings-operation.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

