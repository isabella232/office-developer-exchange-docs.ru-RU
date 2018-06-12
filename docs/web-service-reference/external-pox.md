---
title: Внешние (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: Внешний элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из за пределами сети организации.
ms.openlocfilehash: 7f01fc29b5ce63b02de0a4a6e42887dcffbb4b82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762474"
---
# <a name="external-pox"></a>Внешние (POX)

**Внешний** элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из за пределами сети организации. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Внешние (POX)](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OWAUrl (POX)](owaurl-pox.md) <br/> |Описывает URL-адрес и схемы проверки подлинности, используемый для доступа к на конкретном компьютере, на котором выполняется Microsoft Exchange Server, который имеет роль сервера клиентского доступа установлен, на котором размещается веб-клиент Outlook.  <br/> |
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа. Этот элемент **протокола** имеет только два дочерних элементов: [Тип (POX)](type-pox.md) элемент, указывающий протокол подключения и элемент управления [ASUrl (POX)](asurl-pox.md) , определяющее конечной точки веб-служб Exchange для обеспечения доступности веб-службы.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="remarks"></a>Замечания

**Внешний** элемент является необязательным дочерним элементом элемента **протокола** . 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

