---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: Элемент AllowExternalOof содержит значение, указывающее которому отправляются внешних сообщений об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761374"
---
# <a name="allowexternaloof"></a>AllowExternalOof

Элемент **AllowExternalOof** содержит значение, указывающее которому отправляются внешних сообщений об отсутствии на работе Office (отсутствие на работе). 
  
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
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Содержит параметры об отсутствии на работе для пользователя и результатов ответа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|**None** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправлять сообщения пользователю, не получат внешнего ответа сообщение об отсутствии на работе.  <br/> |
|**Известные** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, которые отправляют сообщения, чтобы пользователь получит только внешние ответа сообщение об отсутствии на работе Если отправитель входит в Exchange пользователя хранить список контактов.  <br/> |
|**All** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправлять сообщения для пользователя будет получать внешние ответа сообщение об отсутствии на работе.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент использует совместно с типом элемента [ExternalAudience](externalaudience.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserOofSettings](getuseroofsettings-operation.md) 
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

