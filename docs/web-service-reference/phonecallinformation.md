---
title: PhoneCallInformation
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
description: Элемент PhoneCallInformation определяет сведения о состоянии для телефонного звонка.
ms.openlocfilehash: e64e7b38b3801c60df8a966e95d980746533d3a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834758"
---
# <a name="phonecallinformation"></a>PhoneCallInformation

Элемент **PhoneCallInformation** определяет сведения о состоянии для телефонного звонка. 
  
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
|[SIPResponseText](sipresponsetext.md) <br/> |Задает текст ответа SIP. Этот элемент является необязательным.  <br/> |
|[SIPResponseCode](sipresponsecode.md) <br/> |Задает код ответа SIP. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetPhoneCallInformationResponse](getphonecallinformationresponse.md) <br/> |Определяет ответ на запрос [GetPhoneCallInformation операции](getphonecallinformation-operation.md) .  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

