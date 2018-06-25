---
title: GetFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolderResponseMessage
api_type:
- schema
ms.assetid: 51359863-d110-4c12-b89f-aba5e3e40c1d
description: Элемент GetFolderResponseMessage содержит состояние и результат одного запроса GetFolder операции.
ms.openlocfilehash: a6b67907dba311a3ce482ff8f524378fb4be9694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762798"
---
# <a name="getfolderresponsemessage"></a>GetFolderResponseMessage

Элемент **GetFolderResponseMessage** содержит состояние и результат одного запроса [GetFolder операции](getfolder-operation.md) . 
  
- [GetFolderResponse](getfolderresponse.md) 
- [ResponseMessages](responsemessages.md)
- [GetFolderResponseMessage](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 **FolderInfoResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описание состояния ответа [GetFolder операции](getfolder-operation.md) . <br/><br/>Для этого атрибута допустимы следующие значения:<br/>  <br/>-Success  <br/>-Предупреждение  <br/>-Ошибка  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Успех** <br/> |Описание запроса, который будет выполнен.  <br/> |
|**Предупреждение** <br/> | Описание запроса, который не был обработан. Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать. <br/><br/>Ниже приведены примеры источников предупреждений:  <br/><br/>-В хранилище Exchange будут недоступны во время пакета.  <br/>-Доменных служб active Directory (AD DS) находится в автономном режиме.  <br/>-Почтовые ящики перемещаются.  <br/>-База данных сообщений (MDB) находится в автономном режиме.  <br/>-Пароль просрочен.  <br/>-Превышено квоту.  <br/> |
|**Error** <br/> | Описание запроса, который не может быть выполнен. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>-Недопустимый атрибуты и элементы  <br/>-Атрибуты или элементы вне диапазона  <br/>— Неизвестный тег  <br/>-Атрибут или элемент не допускается в контексте  <br/>— Попытка доступа не санкционировано любой клиент  <br/>-Сбой сервере в ответ на допустимый вызовов со стороны клиента  <br/><br/>  Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Текст с описанием состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользуемых и зарезервирован для будущего использования. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
|[Папки](folders-ex15websvcsotherref.md) <br/> |Содержит набор папок, используемых в операциях папки.  <br/> |
   
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

- [GetFolder](getfolder.md)
- [GetFolderResponse](getfolderresponse.md) 
- [GetFolder Operation](getfolder-operation.md)

