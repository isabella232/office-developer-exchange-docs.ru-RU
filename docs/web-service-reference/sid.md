---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: Элемент SID представляет язык определения дескриптора безопасности (SDDL) идентификатора безопасности (SID) для учетной записи, используемой для олицетворения или делегирования доступа.
ms.openlocfilehash: 436f284b59d5146b481a25b7b0986db4aeee67ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547059"
---
# <a name="sid"></a>SID

Элемент **SID** представляет язык определения дескриптора безопасности (SDDL) идентификатора безопасности (SID) для учетной записи, используемой для олицетворения или делегирования доступа. 
  
```xml
<SID/>
```

 **SIDType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Представляет учетную запись для олицетворения при использовании загона SOAP ExchangeImpersonation.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[UserId](userid.md) <br/> |Идентифицирует пользователя делегирования или пользователя с разрешениями доступа к папке.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет строковое представление SID.
  
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, который Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

