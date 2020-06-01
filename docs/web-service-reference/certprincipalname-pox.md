---
title: ЦертпринЦипалнаме (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: Элемент ЦертпринЦипалнаме указывает имя участника сертификата SSL, необходимое для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL.
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463344"
---
# <a name="certprincipalname-pox"></a>ЦертпринЦипалнаме (POX)

Элемент **цертпринЦипалнаме** указывает имя участника сертификата SSL, необходимое для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[ЦертпринЦипалнаме (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на котором работает Exchange 2007, на котором установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает имя субъекта сертификата SSL, которое требуется для подключения к организации Microsoft Exchange с помощью протокола SSL.
  
## <a name="remarks"></a>Примечания

Если элемент **цертпринЦипалнаме** не указан, по умолчанию задается значение МССТД: Server, где Server — это значение, указанное в элементе [Server (POX)](server-pox.md) . Например, если параметр SERVER указан как example.com, а **цертпринЦипалнаме** остается пустым с включенным [протоколом SSL (POX)](ssl-pox.md) , значение по умолчанию **цертпринЦипалнаме** будет мсстд:ексампле. com. 
  
Если **этот параметр не** указан, Windows будет проверять имя субъекта сертификата в соответствии с информацией, которая находится в разделе " [имена субъектов](https://go.microsoft.com/fwlink/?LinkId=93417) " на сайте MSDN. 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

