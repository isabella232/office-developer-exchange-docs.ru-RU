---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: Элемент AuthPackage указывает схему проверки подлинности, используемую при проверке подлинности Exchange сервера, на который установлена роль сервера почтовых ящиков.
ms.openlocfilehash: aff4e84cd44d76c2c5a913b6627e1b0c87bab4dc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513026"
---
# <a name="authpackage-pox"></a>AuthPackage (POX)

Элемент **AuthPackage** указывает схему проверки подлинности, используемую при проверке подлинности на сервере Exchange, на который установлена роль сервера почтовых ящиков. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает схему проверки подлинности, которая используется при проверке подлинности на сервере почтовых ящиков. Ниже перечислены возможные значения.
  
- основные
- kerb
- kerbntlm
- ntlm
- certificate
- согласование
- nego2
    
## <a name="remarks"></a>Заметки

Элемент **AuthPackage** используется только в том случае, если элемент [Type (POX)](type-pox.md) имеет текстовое значение EXCH или EXPR. 
  
### <a name="version-differences"></a>Различия версий

Office 365, Exchange Online и локальной версии Exchange, начиная со сборки 15.00.0995.014, возвращают значение "согласование", только если сервер настроен на использование проверки подлинности Negotiate и клиент включает в себя загонщик [X-ClientCanHandle,](pox-autodiscover-request-for-exchange.md) содержащий "Negotiate". 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

