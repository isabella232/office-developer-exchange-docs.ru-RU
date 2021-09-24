---
title: ServerVersionInfo (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: Элемент ServerVersionInfo содержит версию сервера, обрабатываемого запросом.
ms.openlocfilehash: ac52b3eda429e65cb1ec046167a63fe4029d423a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521458"
---
# <a name="serverversioninfo-soap"></a>ServerVersionInfo (SOAP)

Элемент **ServerVersionInfo содержит** версию сервера, обрабатываемого запросом. 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 **ServerVersionInfo**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MajorVersion (SOAP)](majorversion-soap.md) <br/> |Основной номер версии для сервера.  <br/> |
|[MinorVersion (SOAP)](minorversion-soap.md) <br/> |Небольшой номер версии для сервера.  <br/> |
|[MajorBuildNumber (SOAP)](majorbuildnumber-soap.md) <br/> |Основной номер сборки для сервера.  <br/> |
|[MinorBuildNumber (SOAP)](minorbuildnumber-soap.md) <br/> |Небольшой номер сборки для сервера.  <br/> |
|[Version (SOAP)](version-soap.md) <br/> |Описание версии продукта сервера.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Этот элемент возвращается в загона SOAP.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

