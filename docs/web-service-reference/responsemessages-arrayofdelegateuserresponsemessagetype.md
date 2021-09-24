---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: Элемент ResponseMessages содержит сообщения отклика для запроса Exchange управления веб-службами.
ms.openlocfilehash: aa90d2572679ecf3e5d99cc55731d388e083ff01
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525569"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

Элемент **ResponseMessages содержит** сообщения отклика для запроса управления Exchange веб-служб. 
  
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
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Содержит сообщения отклика для операций управления делегированием.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Содержит состояние и результат запроса [операции AddDelegate.](adddelegate-operation.md)  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Содержит состояние и результат запроса на операцию [GetDelegate.](getdelegate-operation.md)  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Содержит состояние и результат запроса на операцию [UpdateDelegate.](updatedelegate-operation.md)  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Содержит состояние и результат запроса [на операцию RemoveDelegate.](removedelegate-operation.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент используется в операции [AddDelegate,](adddelegate-operation.md) [операции GetDelegate,](getdelegate-operation.md)операции [UpdateDelegate](updatedelegate-operation.md)и [операции RemoveDelegate.](removedelegate-operation.md) Ответы на операции управления делегатами структурированы иначе, чем другие ответы. Сообщения ответов управления делегатами строго введите.
  
Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, который Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция AddDelegate](adddelegate-operation.md)
  
[Операция GetDelegate](getdelegate-operation.md)
  
[Операция UpdateDelegate](updatedelegate-operation.md)
  
[Операция RemoveDelegate](removedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

