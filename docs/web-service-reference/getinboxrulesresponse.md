---
title: GetInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetInboxRulesResponse
api_type:
- schema
ms.assetid: 6d6c1950-c328-489a-94bf-a250fdbd5cd9
description: Элемент GetInboxRulesResponse определяет ответ на запрос операции GetInboxRules.
ms.openlocfilehash: e2d3b186922c2a61feb0a2c13fbaa3d02dbdd953
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520551"
---
# <a name="getinboxrulesresponse"></a>GetInboxRulesResponse

Элемент **GetInboxRulesResponse** определяет ответ на запрос [операции GetInboxRules.](getinboxrules-operation.md) 
  
```XML
<GetInboxRulesResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <OutlookRuleBlobExists/>
   <InboxRules/>
</GetInboxRulesResponse>
```

 **GetInboxRulesResponseType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа на операцию [GetInboxRules.](getinboxrules-operation.md) <br/><br/>Для данного атрибута допустимы следующие значения: <br/> <br/>–  Success  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов. <br/><br/>Ниже приведены примеры источников предупреждений:  <br/><br/>– Хранилище Exchange находится в автономном режиме при обработке пакета.  <br/>– Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>– Почтовые ящики перемещены.  <br/>– База данных сообщений (MDB) находится в автономном режиме.  <br/>– Срок действия пароля истек.  <br/>– Превышена квота  <br/> |
|**Error** <br/> | Описывает запрос, который невозможно выполнить. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>– Недопустимые атрибуты или элементы  <br/>- Атрибуты или элементы, которые находятся вне диапазона  <br/>- Неизвестный тег  <br/>— атрибут или элемент, не допустимый в контексте  <br/>- Несанкционированная попытка доступа любого клиента  <br/>- Сбой на стороне сервера в ответ на допустимый клиентский вызов  <br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет сведения о состоянии запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[OutlookRuleBlobExists](outlookruleblobexists.md) <br/> |Указывает, существует ли Outlook правила Майкрософт в почтовом ящике пользователя.  <br/> |
|[InboxRules](inboxrules.md) <br/> |Представляет массив правил в почтовом ящике пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [GetInboxRules](getinboxrules.md)
- [Операция GetInboxRules](getinboxrules-operation.md)

