---
title: упдатеделегатереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegateResponse
api_type:
- schema
ms.assetid: cd336add-fbcc-4f61-9867-d4c08a60e142
description: Элемент Упдатеделегатереспонсе содержит состояние и результат запроса операции UpdateDelegate.
ms.openlocfilehash: 9f11d87ac07dd51a5231d4546fac92e7ca95ad4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465053"
---
# <a name="updatedelegateresponse"></a>упдатеделегатереспонсе

Элемент **упдатеделегатереспонсе** содержит состояние и результат запроса [операции UpdateDelegate](updatedelegate-operation.md) . 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 **упдатеделегатереспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.  <br/> |
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для последующего использования. Он содержит значение 0.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateDelegate](updatedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

