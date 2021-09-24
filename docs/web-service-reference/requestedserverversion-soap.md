---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: Элемент RequestedServerVersion указывает серверную версию, на которую направлен вызов метода автооткрытия.
ms.openlocfilehash: 0690481523ab48497c40338a8808dfa2ed9b0e99
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540561"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

Элемент **RequestedServerVersion** указывает серверную версию, на которую **направлен** вызов метода автооткрытия. 
  
```XML
<RequestedServerVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **RequestedServerVersion** указывает серверную  версию, на которую направлен вызов метода автооткрытия. В следующей таблице перечислены допустимые версии сервера. 
  
|**Текстовое значение**|**Описание**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Пакет обновления 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010 г.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Пакет обновления 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Пакет обновления 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013 г. Поле Exchange2013 применимо для клиентов, которые Exchange Online и версии Exchange начиная с Exchange Server 2013 года.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Пакет обновления 1 (SP1). Поле Exchange2013_SP1 применимо для клиентов, которые Exchange Online и версии Exchange, начиная с Exchange Server 2013 sp1.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **RequestedServerVersion** установлен в загонах SOAP. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

