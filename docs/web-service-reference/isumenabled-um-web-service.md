---
title: IsUMEnabled (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: Элемент IsUMEnabled указывает, включен ли для почтового ящика единая система обмена сообщениями.
ms.openlocfilehash: ea5bde677c62664acad8afd5c8142e96d82b7a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458231"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (веб-служба единой системы обмена сообщениями)

Элемент **IsUMEnabled** указывает, включен ли для почтового ящика единая система обмена сообщениями. 
  
```xml
<IsUMEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Если этот элемент включен, необходимо указать текстовое значение, представляющее логическое значение. Значение **true** указывает на то, что для почтового ящика включена поддержка единой системы обмена сообщениями. Значение **false** означает, что для почтового ящика не включена поддержка единой системы обмена сообщениями. 
  
## <a name="remarks"></a>Примечания

Чтобы определить, включен ли для почтового ящика единая система обмена сообщениями, используйте [операцию IsUMEnabled (веб-служба единой системы обмена](isumenabled-operation-um-web-service.md)сообщениями).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)](isumenabled-operation-um-web-service.md)


[XML-элементы веб-службы единой системы обмена сообщениями для Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

