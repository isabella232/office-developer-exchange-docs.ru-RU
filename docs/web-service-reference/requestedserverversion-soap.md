---
title: Рекуестедсерверверсион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: Элемент Рекуестедсерверверсион указывает версию сервера, для которой вызывается метод автообнаружения.
ms.openlocfilehash: ff63c82943bdd3476a4284f5aa2075fc9c0194b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467909"
---
# <a name="requestedserverversion-soap"></a>Рекуестедсерверверсион (SOAP)

Элемент **рекуестедсерверверсион** указывает версию сервера, для которой вызывается метод **автообнаружения** . 
  
```XML
<RequestedServerVersion/>
```

 **ексчанжеверсион**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **рекуестедсерверверсион** указывает версию сервера, для которой вызывается метод **автообнаружения** . В следующей таблице приведены допустимые версии серверов. 
  
|**Текстовое значение**|**Описание**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 с пакетом обновления 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 с пакетом обновления 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. Поле Exchange2013 применяется для клиентов, которые ориентированы на Exchange Online и версии Exchange, начиная с Exchange Server 2013.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 с пакетом обновления 1 (SP1). Поле Exchange2013_SP1 подходит для клиентов, которые ориентированы на Exchange Online и версии Exchange, начиная с Exchange Server 2013 с пакетом обновления 1 (SP1).  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **рекуестедсерверверсион** задается в заголовке SOAP. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

