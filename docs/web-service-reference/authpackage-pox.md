---
title: Ауспаккаже (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: Элемент Ауспаккаже указывает схему проверки подлинности, используемую при проверке подлинности на сервере Exchange, на котором установлена роль сервера почтовых ящиков.
ms.openlocfilehash: 5317cf49d354a558417829e1d1b5b67cd6874309
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459106"
---
# <a name="authpackage-pox"></a>Ауспаккаже (POX)

Элемент **ауспаккаже** указывает схему проверки подлинности, используемую при проверке подлинности на сервере Exchange, на котором установлена роль сервера почтовых ящиков. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)
  
- [Ответ (POX)](response-pox.md)
  
- [Учетная запись (POX)](account-pox.md)
  
- [Протокол (POX)](protocol-pox.md)
  
- [Ауспаккаже (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
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
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает схему проверки подлинности, используемую при проверке подлинности на сервере почтовых ящиков. Ниже перечислены возможные значения.
  
- Основное
- Kerbtray
- кербнтлм
- NTLM
- certificate
- подключение
- nego2
    
## <a name="remarks"></a>Примечания

Элемент **ауспаккаже** используется только в том случае, когда элемент [Type (POX)](type-pox.md) имеет текстовое значение в формате "курс" или "expr". 
  
### <a name="version-differences"></a>Различия версий

Office 365, Exchange Online и локальная версия Exchange, начиная с сборки 15.00.0995.014, возвращают значение "Negotiate" только в том случае, если сервер настроен на использование проверки подлинности согласования, а клиент включает заголовок [X-клиентканхандле](pox-autodiscover-request-for-exchange.md) , который содержит "Negotiate". 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

