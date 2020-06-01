---
title: финдпеоплереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: Элемент Финдпеоплереспонсе указывает ответ на запрос FindPeople.
ms.openlocfilehash: b969ac3f7bc2bbd3fc77bf753a15696c3b6d8216
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466404"
---
# <a name="findpeopleresponse"></a>финдпеоплереспонсе

Элемент **финдпеоплереспонсе** указывает ответ на запрос **FindPeople** . 
  
```XML
<FindPeopleResponse ResponseClass=" Success | Warning | Error ">
    <People/>
    <TotalNumberOfPeopleInView/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindPeopleResponse>
```

 **финдпеоплереспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|респонсекласс  <br/> |Указывает класс ответа.  <br/> |
   
#### <a name="responseclass"></a>респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|Успешно  <br/> |Указывает на успешное выполнение.  <br/> |
|Предупреждение  <br/> |Указывает на предупреждение.  <br/> |
|Ошибка  <br/> |Указывает на ошибку.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Люди](people.md) <br/> |Указывает массив данных о пользователях, возвращаемых в результате запроса **FindPeople** .  <br/> |
|[тоталнумберофпеоплеинвиев](totalnumberofpeopleinview.md) <br/> |Указывает общее количество пользователей, хранящихся на сервере, которые возвращаются запросом **FindPeople** .  <br/> |
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет сведения о состоянии запроса.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для будущего использования.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Указывает массив ответных сообщений.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

