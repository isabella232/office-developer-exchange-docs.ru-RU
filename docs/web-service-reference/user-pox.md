---
title: Пользователь (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: Элемент User предоставляет сведения о пользователе.
ms.openlocfilehash: 3f90ff0cc00170170c7304f2a19fe1d7abd9d1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840408"
---
# <a name="user-pox"></a>Пользователь (POX)

Элемент **User** предоставляет сведения о пользователе. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Пользователь (POX)](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Отображаемое имя (строка)](displayname-string.md) <br/> |Представляет отображаемое имя пользователя.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Определяет, устаревшее различающееся имя почтового ящика пользователя.  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |Уникально идентифицирует лес Exchange.  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |Содержит SMTP-адрес пользователя, который используется для процесса автообнаружения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ответ (POX)](response-pox.md) <br/> |Содержит ответ от службы автообнаружения.  <br/> |
   
## <a name="remarks"></a>Замечания

Автообнаружение запросы и ответы значения кодировке UTF-8.
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

