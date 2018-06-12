---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: Элемент RequestedServerVersion указывает метод автообнаружения обзвона версии сервера.
ms.openlocfilehash: 6b9d31f3b7bca087652f04e4943becc5ac4e68e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835132"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

Элемент **RequestedServerVersion** указывает метод **автообнаружения** обзвона версии сервера. 
  
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

Текстовое значение элемента **RequestedServerVersion** указывает версию сервера, метод **автообнаружения** обзвона. В следующей таблице приведены версии допустимого сервера. 
  
|**Текстовое значение**|**Описание**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 с пакетом обновления 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 с пакетом обновления 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. В поле Exchange2013 используется для клиентов, относящихся к Exchange Online и версии Exchange, начиная с Exchange Server 2013.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 с пакетом обновления 1 (SP1). В поле Exchange2013_SP1 используется для клиентов, относящихся к Exchange Online и версии Exchange, начиная с Exchange Server 2013 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **RequestedServerVersion** устанавливается в заголовке SOAP. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

