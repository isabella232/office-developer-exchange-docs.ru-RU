---
title: Жетусерсеттингсреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: Элемент Жетусерсеттингсреспонсе представляет ответ на запрос операции GetUserSettings (SOAP).
ms.openlocfilehash: a41a195a003789ddaef81f844e47aad689df0937
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530150"
---
# <a name="getusersettingsresponse-soap"></a>Жетусерсеттингсреспонсе (SOAP)

Элемент **жетусерсеттингсреспонсе** представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) . 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 **жетусерсеттингсреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращенный службой автообнаружения.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.  <br/> |
|[Усерреспонсес (SOAP)](userresponses-soap.md) <br/> |Содержит параметры конфигурации для каждого запрошенного пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)

