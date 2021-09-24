---
title: PhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: Элемент PhoneCallInformation указывает сведения о состоянии для телефонного звонка.
ms.openlocfilehash: 815e0ffac761b12969483752f5022f8580f6cc62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528328"
---
# <a name="phonecallinformation"></a>PhoneCallInformation

Элемент **PhoneCallInformation** указывает сведения о состоянии для телефонного звонка. 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 **PhoneCallInformationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PhoneCallState](phonecallstate.md) <br/> |Указывает состояние для телефонного звонка. Этот элемент обязательный.  <br/> |
|[ConnectionFailureCause](connectionfailurecause.md) <br/> |Указывает причину сбоя подключения. Этот элемент обязательный.  <br/> |
|[SIPResponseText](sipresponsetext.md) <br/> |Указывает текст ответа SIP. Этот элемент является необязательным.  <br/> |
|[SIPResponseCode](sipresponsecode.md) <br/> |Указывает код ответа SIP. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetPhoneCallInformationResponse](getphonecallinformationresponse.md) <br/> |Определяет ответ на запрос [операции GetPhoneCallInformation.](getphonecallinformation-operation.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

