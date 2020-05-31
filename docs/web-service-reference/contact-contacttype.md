---
title: Контактное лицо (Контакттипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: Элемент Contact указывает контакт в едином хранилище контактов.
ms.openlocfilehash: f1593da78a46851c7db43abc567eb66c0c74e0f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761726"
---
# <a name="contact-contacttype"></a>Контактное лицо (Контакттипе)

Элемент **Contact** указывает контакт в едином хранилище контактов. 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 **контакттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PersonName](personname.md) <br/> |Указывает имя пользователя.  <br/> |
|[BusinessName](businessname.md) <br/> |Указывает название организации.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Представляет коллекцию телефонных номеров контакта.  <br/> |
|[Urls](urls.md) <br/> |Указывает массив URL-адресов для пользователя.  <br/> |
|[EmailAddresses (Аррайофекстрактедемаиладдрессес)](emailaddresses-arrayofextractedemailaddresses.md) <br/> |Указывает массив извлеченных адресов электронной почты.  <br/> |
|[Адреса (Аррайофаддрессестипе)](addresses-arrayofaddressestype.md) <br/> |Указывает массив элементов **Address** .  <br/> |
|[контактстринг](contactstring.md) <br/> |Задает отображаемое имя контакта.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Contacts (Аррайофконтактстипе)](contacts-arrayofcontactstype.md) <br/> |Указывает массив контактов.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

