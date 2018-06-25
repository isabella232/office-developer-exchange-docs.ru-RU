---
title: UpdateInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRulesResponse
api_type:
- schema
ms.assetid: 0947b6aa-0d95-421b-aebb-d03021ecc110
description: Элемент UpdateInboxRulesResponse определяет ответ на запрос UpdateInboxRules.
ms.openlocfilehash: cd64e4546f8d9bf573062d9c982477be3fa4d925
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840346"
---
# <a name="updateinboxrulesresponse"></a>UpdateInboxRulesResponse

Элемент **UpdateInboxRulesResponse** определяет ответ на запрос UpdateInboxRules. 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 **UpdateInboxRulesResponseType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описание состояния ответа [операции отказа от подписки](unsubscribe-operation.md) .<br/><br/> Для этого атрибута допустимы следующие значения:  <br/><br/>-Success  <br/>-Предупреждение  <br/>-Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Успех** <br/> |Описание запроса, который будет выполнен.  <br/> |
|**Предупреждение** <br/> | Описание запроса, который не был обработан. Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать. <br/><br/>Ниже приведены примеры источников предупреждений:  <br/><br/>-В хранилище Exchange будут недоступны во время пакета.  <br/>-Доменных служб active Directory (AD DS) находится в автономном режиме.  <br/>-Почтовые ящики перемещаются.  <br/>-База данных сообщений (MDB) находится в автономном режиме.  <br/>-Пароль просрочен.  <br/>-Превышено квоту.  <br/> |
|**Error** <br/> | Описание запроса, который не может быть выполнен. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>-Недопустимый атрибуты и элементы  <br/>-Атрибуты или элементы, которые являются вне диапазона  <br/>— Неизвестный тег  <br/>-Атрибута или элемента, который не является допустимым в контексте  <br/>-Попытка несанкционированного доступа с любого клиента  <br/>-Сбой на сервере в ответ на допустимый вызовов со стороны клиента  <br/> <br/> Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет сведения о состоянии о запросе.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользуемых и зарезервирован для будущего использования. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
|[RuleOperationErrors](ruleoperationerrors.md) <br/> |Представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [UpdateInboxRules](updateinboxrules.md)
- [Операция UpdateInboxRules](updateinboxrules-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

