---
title: AddDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegateResponse
api_type:
- schema
ms.assetid: d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429
description: Элемент AddDelegateResponse содержит состояние и результат запроса AddDelegate операции.
ms.openlocfilehash: a1d56e9994b3a7916fe0fbe40be1e6d8ff473730
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761334"
---
# <a name="adddelegateresponse"></a>AddDelegateResponse

Элемент **AddDelegateResponse** содержит состояние и результат [операции AddDelegate](adddelegate-operation.md) запроса. 
  
```xml
<AddDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddDelegateResponse>
```

 **AddDelegateResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages (ArrayOfDelegateUserResponseMessageType)](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |Содержит сообщения ответа на запрос управления delegate веб-служб Exchange.  <br/> |
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользуемых и зарезервирован для будущего использования. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
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

- [Операция AddDelegate](adddelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

