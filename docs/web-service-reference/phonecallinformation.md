---
title: фонекаллинформатион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: Элемент Фонекаллинформатион указывает сведения о состоянии телефонного звонка.
ms.openlocfilehash: 75370bccb841818a8302bdd055ad96fd16b2e8df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468847"
---
# <a name="phonecallinformation"></a>фонекаллинформатион

Элемент **фонекаллинформатион** указывает сведения о состоянии телефонного звонка. 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 **фонекаллинформатионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фонекаллстате](phonecallstate.md) <br/> |Указывает состояние телефонного звонка. Этот элемент обязательный.  <br/> |
|[коннектионфаилурекаусе](connectionfailurecause.md) <br/> |Указывает причину сбоя подключения. Этот элемент обязательный.  <br/> |
|[сипреспонсетекст](sipresponsetext.md) <br/> |Задает текст ответа SIP. Этот элемент является необязательным.  <br/> |
|[сипреспонсекоде](sipresponsecode.md) <br/> |Задает код ответа SIP. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетфонекаллинформатионреспонсе](getphonecallinformationresponse.md) <br/> |Определяет ответ на запрос [операции GetPhoneCallInformation](getphonecallinformation-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

