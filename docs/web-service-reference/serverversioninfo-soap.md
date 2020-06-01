---
title: Серверверсионинфо (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: Элемент Серверверсионинфо содержит версию сервера, который обработал запрос.
ms.openlocfilehash: b54b4833361ec78c7f8213473af4638965c7ddae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467650"
---
# <a name="serverversioninfo-soap"></a>Серверверсионинфо (SOAP)

Элемент **серверверсионинфо** содержит версию сервера, который обработал запрос. 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 **серверверсионинфо**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MajorVersion (SOAP)](majorversion-soap.md) <br/> |Основной номер версии сервера.  <br/> |
|[MinorVersion (SOAP)](minorversion-soap.md) <br/> |Дополнительный номер версии сервера.  <br/> |
|[Мажорбуилднумбер (SOAP)](majorbuildnumber-soap.md) <br/> |Основной номер сборки для сервера.  <br/> |
|[Минорбуилднумбер (SOAP)](minorbuildnumber-soap.md) <br/> |Дополнительный номер сборки для сервера.  <br/> |
|[Версия (SOAP)](version-soap.md) <br/> |Описание версии серверного продукта.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент возвращается в заголовке SOAP.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

