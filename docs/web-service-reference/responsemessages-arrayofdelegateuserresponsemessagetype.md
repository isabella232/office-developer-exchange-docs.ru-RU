---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: Элемент ResponseMessages содержит сообщений ответа на запрос управления delegate веб-служб Exchange.
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

Элемент **ResponseMessages** содержит сообщений ответа на запрос управления delegate веб-служб Exchange. 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfDelegateUserResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Содержит сообщения ответа для операции управления delegate.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Содержит состояние и результат [операции AddDelegate](adddelegate-operation.md) запроса.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Содержит состояние и результат [операции GetDelegate](getdelegate-operation.md) запроса.  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Содержит состояние и результат [операции UpdateDelegate](updatedelegate-operation.md) запроса.  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Содержит состояние и результат [операции RemoveDelegate](removedelegate-operation.md) запроса.  <br/> |
   
## <a name="remarks"></a>Замечания

Данный элемент используется в [операции AddDelegate](adddelegate-operation.md), [GetDelegate операции](getdelegate-operation.md), [операция UpdateDelegate](updatedelegate-operation.md)и [RemoveDelegate операции](removedelegate-operation.md). Ответы операции управления delegate структурированы иначе, чем другие ответы. Сообщения ответа управления delegate строго типизированный.
  
Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция AddDelegate](adddelegate-operation.md)
  
[Операция GetDelegate](getdelegate-operation.md)
  
[Операция UpdateDelegate](updatedelegate-operation.md)
  
[Операция RemoveDelegate](removedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

