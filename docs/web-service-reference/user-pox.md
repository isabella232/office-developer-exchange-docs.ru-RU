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
description: Элемент User предоставляет сведения, относящиеся к пользователю.
ms.openlocfilehash: 8f53319bcf34595305748adafc9aa1e25283611e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530220"
---
# <a name="user-pox"></a>Пользователь (POX)

Элемент **User** предоставляет сведения, относящиеся к пользователю. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
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

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DisplayName (строка)](displayname-string.md) <br/> |Представляет отображаемое имя пользователя.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Определяет почтовый ящик пользователя, используя устаревшее различающееся имя.  <br/> |
|[Деплойментид (POX)](deploymentid-pox.md) <br/> |Уникальный идентификатор леса Exchange.  <br/> |
|[Аутодисковерсмтпаддресс (POX)](autodiscoversmtpaddress-pox.md) <br/> |Содержит SMTP-адрес пользователя, который используется для процесса автообнаружения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ответ (POX)](response-pox.md) <br/> |Содержит ответ от службы автообнаружения.  <br/> |
   
## <a name="remarks"></a>Примечания

Запросы и ответы автообнаружения должны быть закодированы в кодировке UTF 8.
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

