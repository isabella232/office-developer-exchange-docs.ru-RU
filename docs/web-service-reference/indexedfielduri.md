---
title: индекседфиелдури
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: Элемент Индекседфиелдури определяет отдельные элементы словаря.
ms.openlocfilehash: f794d9970590417d916925f7258b28d4f0920d0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467020"
---
# <a name="indexedfielduri"></a>индекседфиелдури

Элемент **индекседфиелдури** определяет отдельные элементы словаря. 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **пастоиндекседфиелдтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**фиелдури** <br/> |Определяет словарь, содержащий возвращаемый член. Этот атрибут является обязательным.  <br/> |
|**фиелдиндекс** <br/> |Определяет возвращаемый элемент словаря. Этот атрибут является обязательным.  <br/> |
   
#### <a name="fielduri-attribute"></a>Атрибут Фиелдури

|**Значение**|**Описание**|
|:-----|:-----|
|элемент: InternetMessageHeader  <br/> |Представляет заголовок сообщения для элемента.  <br/> |
|Контакты: адрес  <br/> |Представляет адрес обмена мгновенными сообщениями контакта.  <br/> |
|Контакты: PhysicalAddress: улица  <br/> |Представляет почтовый адрес контакта.  <br/> |
|Контакты: PhysicalAddress: City  <br/> |Представляет город контакта.  <br/> |
|Контакты: PhysicalAddress: State  <br/> |Представляет состояние контакта.  <br/> |
|Контакты: PhysicalAddress: Country  <br/> |Представляет страну или регион контакта.  <br/> |
|Contacts: PhysicalAddress: PostalCode  <br/> |Представляет почтовый индекс контакта.  <br/> |
|Контакты: PhoneNumber  <br/> |Представляет номер телефона контакта.  <br/> |
|Contacts: EmailAddress  <br/> |Представляет адрес электронной почты контакта.  <br/> |
|дистрибутионлист: Members: Member  <br/> |Представляет члена списка рассылки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аддитионалпропертиес](additionalproperties.md) <br/> |Определяет дополнительные свойства, которые необходимо получить, задать или создать.  <br/> |
|[аггрегатеон](aggregateon.md) <br/> |Представляет свойство, используемое для определения порядка сгруппированных элементов для группового результирующего набора FindItem.  <br/> |
|[GroupBy](groupby.md) <br/> |Указывает произвольное группирование для запросов FindItem.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

