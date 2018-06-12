---
title: Метод AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 646fb994-229e-4d90-8b95-6541191cb3ae
description: Элемент AddDelegate определяет запрос на Добавление делегатов к почтовому ящику. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d1cb0ff3ea68904bf88e346f68afe7c349ae4394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761342"
---
# <a name="adddelegate"></a>Метод AddDelegate

Элемент **AddDelegate** определяет запрос на Добавление делегатов к почтовому ящику. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<AddDelegate>
   <DelegateUsers/>
   <DeliverMeetingRequests/>
   <Mailbox/>
</AddDelegate>
```

 **AddDelegateType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |Содержит идентификаторы делегатов для добавления или обновления в почтовом ящике. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[DeliverMeetingRequests](delivermeetingrequests.md) <br/> |Определяет порядок обработки приглашений на собрания между делегата и участника. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция AddDelegate](adddelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

