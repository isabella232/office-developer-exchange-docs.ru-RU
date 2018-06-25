---
title: CopyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponseMessage
api_type:
- schema
ms.assetid: c82092a9-50ff-4ae1-b819-ebabbf89262b
description: Элемент CopyFolderResponseMessage содержит состояние и результат одного запроса CopyFolder операции.
ms.openlocfilehash: 2bb2b407e0ae6b854d214c4b9d68ac8ed65b2c7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761839"
---
# <a name="copyfolderresponsemessage"></a>CopyFolderResponseMessage

Элемент **CopyFolderResponseMessage** содержит состояние и результат одного запроса [CopyFolder операции](copyfolder-operation.md) . 
  
- [CopyFolderResponse](copyfolderresponse.md) 
- [ResponseMessages](responsemessages.md)  
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 **FolderInfoResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описание состояния ответа [операции CopyFolder](copyfolder-operation.md) .<br/><br/>Для этого атрибута допустимы следующие значения:<br/><br/>-Success  <br/>-Предупреждение  <br/>-Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Успех** <br/> |Описание запроса, который будет выполнен.  <br/> |
|**Предупреждение** <br/> | Описание запроса, который не был обработан. Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.<br/><br/>Ниже приведены примеры источников предупреждений:<br/><br/>-В хранилище Exchange переходит в автономный режим во время пакета.  <br/>-Доменных служб active Directory (AD DS) переходит в автономный режим.  <br/>-Почтовые ящики перемещаются.  <br/>-База данных сообщений (MDB) переходит в автономный режим.  <br/>-Пароль просрочен.  <br/>-Превышено квоту.  <br/> |
|**Error** <br/> | Описание запроса, который не может быть выполнен.<br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>-Недопустимый атрибуты и элементы  <br/>-Атрибуты или элементы вне диапазона  <br/>— Неизвестный тег  <br/>-Атрибут или элемент не допускается в контексте  <br/>-Предпринята попытка любой клиент несанкционированного доступа  <br/>-Сбой сервере в ответ на допустимый вызовов со стороны клиента<br/><br/>Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользуемых и зарезервирован для будущего использования. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
|[Папки](folders-ex15websvcsotherref.md) <br/> |Содержит массив скопированной папки.  <br/> |
   
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

- [Операция CopyFolder](copyfolder-operation.md)
- [Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md) 
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

