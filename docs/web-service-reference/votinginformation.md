---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: Элемент VotingInformation указывает сведения о голосовании в сообщении о голосовании и сообщении запроса на утверждение, в которомApproveandRejectare параметры голосования.
ms.openlocfilehash: 7e5aedddbfe97bba935aa56b3583e2fb8b081320
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543858"
---
# <a name="votinginformation"></a>VotingInformation

Элемент **VotingInformation** указывает сведения о голосовании в сообщении о голосовании и сообщении запроса на утверждение, где параметры "Утверждение" и "Отклонение" являются вариантами голосования. 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 **VotingInformationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[UserOptions](useroptions.md)  |  [VotingResponse](votingresponse.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Сообщение](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Сообщение](message-ex15websvcsotherref.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

