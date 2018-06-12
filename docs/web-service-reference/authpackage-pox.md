---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: Элемент AuthPackage указывает схемы проверки подлинности, используемый при проверке подлинности на сервере Exchange, с установленной ролью сервера почтовых ящиков.
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761526"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

Элемент **AuthPackage** указывает схемы проверки подлинности, используемый при проверке подлинности на сервере Exchange, с установленной ролью сервера почтовых ящиков. 
  
- [Автообнаружение (POX)](autodiscover-pox.md)
  
- [Ответ (POX)](response-pox.md)
  
- [Учетная запись (POX)](account-pox.md)
  
- [Протокол (POX)](protocol-pox.md)
  
- [AuthPackage (POX)](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение определяет схемы проверки подлинности, используемый при проверке подлинности на сервере почтовых ящиков. Ниже перечислены возможные значения.
  
- Базовая
- kerb
- kerbntlm
- NTLM
- certificate
- согласование
- протокол nego2
    
## <a name="remarks"></a>Замечания

Элемент **AuthPackage** используется только в том случае, когда элемент [Типа (POX)](type-pox.md) имеет значение text EXCH или EXPR. 
  
### <a name="version-differences"></a>Различия версий

Office 365, Exchange Online и локальной версии Exchange, начиная с построения 15.00.0995.014 возвращаемое значение «согласование» только в том случае, если сервер настроен на использование проверки подлинности согласование и клиент включает в себя заголовок [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) , содержит «Согласование». 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

