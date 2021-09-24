---
title: User (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: Элемент User предоставляет сведения, определенные пользователю.
ms.openlocfilehash: 832e0a63e75a08406b3aa397ac29ad5aa300cfe0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522410"
---
# <a name="user-pox"></a>User (POX)

Элемент **User** предоставляет сведения, определенные пользователю. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[User (POX)](user-pox.md)
  
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
|[DisplayName (string)](displayname-string.md) <br/> |Представляет отображаемое имя пользователя.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Определяет почтовый ящик пользователя по устаревшему имени.  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |Уникально определяет лес Exchange.  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |Содержит SMTP-адрес пользователя, используемый для процесса автооткрытия.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |Содержит ответ от службы автооткрытия.  <br/> |
   
## <a name="remarks"></a>Заметки

Автоматические запросы и ответы должны быть закодированы в UTF-8.
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

