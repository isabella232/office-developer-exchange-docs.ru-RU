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
description: Элемент ResponseMessages содержит сообщения ответа для запроса на управление делегированием веб-служб Exchange.
ms.openlocfilehash: 6b035f4ee46af1750a275e2c61b2cddea06b37a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465459"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

Элемент **ResponseMessages** содержит сообщения ответа для запроса на управление делегированием веб-служб Exchange. 
  
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
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Содержит ответные сообщения для операций управления делегированием.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Содержит состояние и результат запроса на операцию [AddDelegate.](adddelegate-operation.md)  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Содержит состояние и результат запроса на операцию [GetDelegate.](getdelegate-operation.md)  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Содержит состояние и результат запроса [операции UpdateDelegate.](updatedelegate-operation.md)  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Содержит состояние и результат запроса на операцию [RemoveDelegate.](removedelegate-operation.md)  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент используется в [операциях AddDelegate,](adddelegate-operation.md) [GetDelegate,](getdelegate-operation.md) [UpdateDelegate](updatedelegate-operation.md)и [RemoveDelegate.](removedelegate-operation.md) Реакции на операции управления делегированием структурированы иначе, чем другие ответы. Сообщения ответа на запросы управления делегированием строго типимы.
  
Схема, описывающую этот элемент, расположена в виртуальном каталоге EWS компьютера, на Exchange Server с установленной ролью сервера клиентского доступа.
  
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

