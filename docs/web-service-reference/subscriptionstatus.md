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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840107"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

Элемент **SubscriptionStatus** описывает состояние принудительной подписки. 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 **субскриптионстатустипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[сенднотификатионресулт](sendnotificationresult.md) <br/> |Содержит ответ клиентского приложения на push-уведомления.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ниже приведены возможные текстовые значения для этого элемента:
  
- OK
    
- Отмена подписки
    
## <a name="remarks"></a>Примечания

Этот элемент описывает состояние подписки. Клиентское приложение принудительной подписки отправляет состояние на компьютер, на котором выполняется Exchange 2007, на котором установлена роль сервера клиентского доступа после каждого push-уведомления. Если значение **SubscriptionStatus** равно **Unsubscribe**, сервер клиентского доступа прекратит отправку уведомлений и завершит подписку. Если значение **SubscriptionStatus** равно **ОК**, сервер клиентского доступа продолжит отправлять уведомления.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

