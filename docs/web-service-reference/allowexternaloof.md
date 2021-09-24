---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: Элемент AllowExternalOof содержит значение, которое определяет, кому отправляются внешние сообщения Office (OOF).
ms.openlocfilehash: 7d2e34797af8a9e9d11570a5ea2e618db7630f0c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523226"
---
# <a name="allowexternaloof"></a>AllowExternalOof

Элемент **AllowExternalOof** содержит значение, которое определяет, кому отправляются внешние сообщения Office (OOF). 
  
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
- [AllowExternalOof](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Содержит результаты ответа и параметры OOF для пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|**Нет** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправившие сообщения пользователю, не получат внешнего ответа на сообщение OOF.  <br/> |
|**Известные** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправившие сообщения пользователю, получат внешний ответ на сообщение OOF только в том случае, если отправитель находится в списке контактов Exchange магазина пользователя.  <br/> |
|**Все** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправившие сообщения пользователю, получат внешний ответ на сообщение OOF.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент имеет тот же тип, что и [элемент ExternalAudience.](externalaudience.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserOofSettings](getuseroofsettings-operation.md) 
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

