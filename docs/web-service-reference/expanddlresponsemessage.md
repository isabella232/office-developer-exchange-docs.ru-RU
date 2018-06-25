---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: Элемент ExpandDLResponseMessage содержит состояние и результат одного запроса операция ExpandDL.
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762438"
---
# <a name="expanddlresponsemessage"></a>ExpandDLResponseMessage

Элемент **ExpandDLResponseMessage** содержит состояние и результат одного запроса [ExpandDL операции](expanddl-operation.md) . 
  
- [ExpandDLResponse](expanddlresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

**ExpandDLResponseMessageType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описание состояния ответа [ExpandDL операции](expanddl-operation.md) .<br/><br/>Для этого атрибута допустимы следующие значения: <br/> <br/>-Success  <br/>-Предупреждение  <br/>-Ошибка  <br/> |
|**IndexedPagingOffset** <br/> |Представляет следующий индекс, который следует использовать для следующего запроса при использовании индексированного представления разбиение на страницы.  <br/> |
|**NumeratorOffset** <br/> |Представляет новое значение перечислителя использовать для следующего запроса при использовании просмотров страниц дроби.  <br/> |
|**AbsoluteDenominator** <br/> |Представляет Далее делителя для использования в следующем запросе при выполнении дробная разбиение на страницы.  <br/> |
|**IncludesLastItemInRange** <br/> |Указывает, что дополнительные разбиение на страницы не требуется. Этот атрибут будет значение true, если текущие результаты содержат последнего элемента в запросе.  <br/> |
|**TotalItemsInView** <br/> |Представляет общее число элементов, которые ограничение игнорируется.  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Успех** <br/> |Описание запроса, который будет выполнен.  <br/> |
|**Предупреждение** <br/> | Описание запроса, который не был обработан. Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.<br/><br/> Ниже приведены примеры источников предупреждений:<br/>  <br/>-В хранилище Exchange будут недоступны во время пакета.  <br/>-Доменных служб active Directory (AD DS) находится в автономном режиме.  <br/>-Почтовые ящики перемещаются.  <br/>-Базы данных почтовых ящиков (MDB) находится в автономном режиме.  <br/>-Пароль просрочен.  <br/>-Превышено квоту.  <br/> |
|**Error** <br/> | Описание запроса, который не может быть выполнен.<br/><br/> Ниже приведены примеры источников ошибок:  <br/><br/>-Недопустимый атрибуты и элементы  <br/>-Атрибуты или элементы, которые являются вне диапазона  <br/>— Неизвестный тег  <br/>-Атрибута или элемента, который не является допустимым в контексте  <br/>-Попытка несанкционированного доступа с любого клиента  <br/>-Сбой на сервере в ответ на допустимый вызовов со стороны клиента <br/> <br/>  Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользуемых и зарезервирован для будущего использования. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Содержит массив почтовых ящиков, которые содержатся в списке рассылки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения ответа на запрос веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ExpandDL](expanddl-operation.md)
- [Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

