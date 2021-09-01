---
title: DirectReports
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab88739f-9018-4887-ae46-f1471242628c
description: Элемент DirectReports содержит сведения SMTP, идентифицирующие прямые отчеты контакта.
ms.openlocfilehash: 216f6e99a3caf46f9d3bc792dcb4641c3681a9fb
ms.sourcegitcommit: 63e48eaf2891a6db1a718b55cd69e3a0433c4a9c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2021
ms.locfileid: "58851109"
---
# <a name="directreports"></a>DirectReports

Элемент **DirectReports содержит** сведения SMTP, идентифицирующие прямые отчеты контакта. 
  
```XML
<DirectReports>
   <Mailbox/>
</DirectReports>
```

 **SingleRecipientType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
     
### <a name="parent-elements"></a>Родительские элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Представляет контактный элемент в Exchange магазине.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание контактов (Exchange веб-служб)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

