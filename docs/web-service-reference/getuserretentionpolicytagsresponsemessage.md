---
title: GetUserRetentionPolicyTagsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9991d6e0-8c31-4e73-8af3-da4298474b66
description: Элемент GetUserRetentionPolicyTagsResponseMessage указывает сообщение ответа на запрос GetUserRetentionPolicyTags.
ms.openlocfilehash: db73cb7f1922d845c9565753ff8d4917b82b1259
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2018
ms.locfileid: "19833701"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a>GetUserRetentionPolicyTagsResponseMessage

Элемент **GetUserRetentionPolicyTagsResponseMessage** указывает сообщение ответа на запрос **GetUserRetentionPolicyTags** . 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 **GetUserRetentionPolicyTagsResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)
  
### <a name="parent-elements"></a>Родительские элементы

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

