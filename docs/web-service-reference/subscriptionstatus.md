---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: Элемент SubscriptionStatus описывает состояние принудительной подписки.
ms.openlocfilehash: 1f6de15f7a3b07714899aef2ff74a8d556f8ca1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840107"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

Элемент **SubscriptionStatus** описывает состояние принудительной подписки. 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 **SubscriptionStatusType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SendNotificationResult](sendnotificationresult.md) <br/> |Содержит ответ в клиентском приложении "для push-уведомлений.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Ниже приведены возможные значения для этого элемента.
  
- OK
    
- Отмена подписки
    
## <a name="remarks"></a>Замечания

В этом элементе представлено описание состояния подписки. Клиентское приложение подписки push отправляет состояние на компьютер, на котором работает Exchange 2007, который имеет роль сервера клиентского доступа, установленные после каждого push-уведомлений. Если значение **SubscriptionStatus** равно **отказа от подписки**, сервер клиентского доступа Остановить отправку уведомлений и end подписки. Если значение **SubscriptionStatus** равно **ОК**, сервер клиентского доступа будет продолжать отправлять уведомления.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

