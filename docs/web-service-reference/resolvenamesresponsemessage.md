---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: Элемент ResolveNamesResponseMessage содержит состояние и результат операции запроса ResolveNames.
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835170"
---
# <a name="resolvenamesresponsemessage"></a>ResolveNamesResponseMessage

Элемент **ResolveNamesResponseMessage** содержит состояние и результат [операции ResolveNames](resolvenames-operation.md) запроса. 
  
- [ResolveNamesResponse](resolvenamesresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 **ResolveNamesResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описание состояния ответа [операции ResolveNames](resolvenames-operation.md) . <br/><br/>Для этого атрибута допустимы следующие значения:  <br/><br/>-Success  <br/>-Предупреждение  <br/>-Ошибка  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Успех** <br/> |Описание запроса, который будет выполнен. Происходит, когда запрошенный имя однозначно идентифицируемый и ответ содержит одного получателя.  <br/> |
|**Предупреждение** <br/> | Описание запроса, который не был обработан. Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать. <br/><br/>Вот пример источников предупреждений:  <br/><br/>-В хранилище Exchange переходит в автономный режим во время пакета.  <br/>-Доменных служб active Directory (AD DS) переходит в автономный режим.  <br/>-Почтовые ящики перемещаются.  <br/>-Базы данных почтовых ящиков (MDB) переходит в автономный режим.  <br/>-Пароль просрочен.  <br/>-Превышено квоту.  <br/>— Имя запрошенного является неоднозначным и ответ содержит несколько получателей.  <br/> |
|**Error** <br/> | Описание запроса, который не может быть выполнен. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>-Указанное имя не может быть разрешен.  <br/>-Атрибуты или элементы являются недопустимыми.  <br/>-Атрибуты или элементы находятся вне диапазона.  <br/>-Неизвестно тег.  <br/>-Атрибута или элемента не является допустимым в контексте.  <br/>-Произошла попытка несанкционированного доступа с любого клиента.  <br/>-На сервере сбой в ответ на допустимый вызовов со стороны клиента.  <br/>  <br/>Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет сведения о запросе.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользуемых и зарезервирован для будущего использования. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
|[ResolutionSet](resolutionset.md) <br/> |Содержит набор разрешений для разрешения неоднозначных псевдонимов.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения ответа на запрос веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [ResolveNames](resolvenames.md)
- [ResolveNamesResponse](resolvenamesresponse.md)
- [Операция ResolveNames](resolvenames-operation.md)

