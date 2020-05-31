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
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761676"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на котором работает Exchange 2007, на котором установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает имя субъекта сертификата SSL, которое требуется для подключения к организации Microsoft Exchange с помощью протокола SSL.
  
## <a name="remarks"></a>Примечания

Если элемент **цертпринЦипалнаме** не указан, по умолчанию задается значение МССТД: Server, где Server — это значение, указанное в элементе [Server (POX)](server-pox.md) . Например, если параметр SERVER указан как example.com, а **цертпринЦипалнаме** остается пустым с включенным [протоколом SSL (POX)](ssl-pox.md) , значение по умолчанию **цертпринЦипалнаме** будет мсстд:ексампле. com. 
  
Если **этот параметр не** указан, Windows будет проверять имя субъекта сертификата в соответствии с информацией, которая находится в разделе " [имена субъектов](http://go.microsoft.com/fwlink/?LinkId=93417) " на сайте MSDN. 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

