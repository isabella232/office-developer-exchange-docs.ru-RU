---
title: MSExchangeCertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c514f22f-be3e-4cad-ac56-bdff6bafcee6
description: Элемент MSExchangeCertificate содержит значение, которое кодирует сертификата Microsoft Exchange контакта.
ms.openlocfilehash: 8d07198012485b5c6d22e1fb4721890bf9a5eb39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834498"
---
# <a name="msexchangecertificate"></a>MSExchangeCertificate

Элемент **MSExchangeCertificate** содержит значение, которое кодирует сертификата Microsoft Exchange контакта. 
  
```XML
<MSExchangeCertificate/>
```

 **ArrayOfBinaryType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[Base64Binary](base64binary.md) <br/> |Содержит значения кодировке Base64.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[Контакт](contact.md) <br/> |Представляет контакт в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание контактов (веб-служб Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

