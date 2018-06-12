---
title: CreateUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 9c11427c-74c9-4c6a-a0e7-7d5556670c1e
description: Элемент CreateUserConfigurationResponseMessage содержит состояние и результат одного запроса CreateUserConfiguration.
ms.openlocfilehash: 718d62d9f5b920eaf9481054b095958a9f44cbf8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761934"
---
# <a name="createuserconfigurationresponsemessage"></a>CreateUserConfigurationResponseMessage

Элемент **CreateUserConfigurationResponseMessage** содержит состояние и результат одного запроса **CreateUserConfiguration** . 
  
```xml
<CreateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</CreateUserConfigurationResponseMessage>
```

**ResponseMessageType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описание состояния ответа.<br/><br/>Для этого атрибута допустимы следующие значения:  <br/><br/>-Success  <br/>-Предупреждение  <br/>-Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Успех** <br/> |Описание запроса, который будет выполнен.  <br/> |
|**Предупреждение** <br/> | Описание запроса, который не был обработан. Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.<br/><br/> Ниже приведены примеры источников предупреждений:  <br/><br/>-В хранилище Exchange будут недоступны во время пакета.  <br/>-Доменных служб active Directory (AD DS) находится в автономном режиме.  <br/>-Почтовые ящики были перемещены.  <br/>-База данных сообщений (MDB) находится в автономном режиме.  <br/>-Пароль просрочен.  <br/>-Квоту превышена.  <br/> |
|**Error** <br/> | Описание запроса, который не может быть выполнен.<br/><br/> Ниже приведены примеры источников ошибок:  <br/><br/>-Недопустимых атрибутов и элементов.  <br/>-Атрибуты или элементы, которые являются вне диапазона.  <br/>— Неизвестный тег.  <br/>-Атрибут или элемент не является допустимым в контексте.  <br/>-При попытке несанкционированного доступа с любого клиента.  <br/>-На сервере сбой в ответ на допустимый вызовов со стороны клиента.<br/><br/>  Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время используется и зарезервировано для будущего использования. Этот элемент содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения ответа на запрос веб-служб Exchange.  <br/> |
   
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

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

