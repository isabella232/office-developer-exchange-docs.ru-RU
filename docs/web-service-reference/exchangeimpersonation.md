---
title: ExchangeImpersonation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: Элемент ExchangeImpersonation используется в заголовке SOAP запроса. Если этот элемент, вызывающего абонента пытается олицетворить учетную запись, которая содержится в элементе ExchangeImpersonation.
ms.openlocfilehash: aedeff22cda865ce1eec80dab9760d49fdc178f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762415"
---
# <a name="exchangeimpersonation"></a>ExchangeImpersonation

Элемент **ExchangeImpersonation** используется в заголовке SOAP запроса. Если этот элемент, вызывающего абонента пытается олицетворить учетную запись, которая содержится в элементе **ExchangeImpersonation** . 
  
[ExchangeImpersonation](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 **ExchangeImpersonationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Вызывающий учетная запись должна иметь **ms-exch-impersonation** непосредственно на сервер клиентского доступа и **ms-exch-MayImpersonate** непосредственно в либо базы данных почтовых ящиков, почтовых ящиков для олицетворения или пользователей/контакт Active Directory объект. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Сервер сервер авторизации в веб-служб Exchange](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

