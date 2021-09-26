---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: Элемент SubscriptionStatus описывает состояние push-подписки.
ms.openlocfilehash: 6918a4965da2c075341c99581c3bd06c93da35fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546933"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

Элемент **SubscriptionStatus** описывает состояние push-подписки. 
  
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
|[SendNotificationResult](sendnotificationresult.md) <br/> |Содержит ответ клиентского приложения на push-уведомление.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Возможные текстовые значения для этого элемента:
  
- OK
    
- Unsubscribe
    
## <a name="remarks"></a>Заметки

Этот элемент описывает состояние подписки. Клиентское приложение push-подписки возвращает состояние на компьютер, который работает Exchange 2007 г., где после каждого push-уведомления устанавливается роль сервера клиентского доступа. Если значение **SubscriptionStatus** равно подписке, сервер клиентского доступа прекратит отправку уведомлений и завершит подписку. Если значение **SubscriptionStatus** равно **ОК,** сервер клиентского доступа будет продолжать отправлять уведомления.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

