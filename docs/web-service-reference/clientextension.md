---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: Элемент ClientExtension содержит пользователей и конфигурации сведения о приложении.
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761684"
---
# <a name="clientextension"></a>ClientExtension

Элемент **ClientExtension** содержит пользователей и конфигурации сведения о приложении. 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 **ClientExtensionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|IsAvailable  <br/> |Указывает, доступна ли приложение. Текстовое значение **true** для атрибута **IsAvailable** указывает, что приложение доступно. Значение **false** указывает, что приложение недоступно. Этот атрибут является необязательным.  <br/> |
|IsMandatory  <br/> |Указывает, будет ли приложение является обязательным. Текстовое значение **true** для атрибута **IsMandatory** указывает, что приложение является обязательным для почтового ящика. Значение **false** указывает, что приложение не является обязательным. Этот атрибут является необязательным.  <br/> |
|IsEnabledByDefault  <br/> |Указывает, включена ли приложение по умолчанию. Текстовое значение **true** для атрибута **IsEnabledByDefault** указывает, что приложение включено по умолчанию. Значение **false** указывает, что приложение не включен по умолчанию. Этот атрибут является необязательным.  <br/> |
|ProvidedTo  <br/> |Указывает, к которому предоставляется приложения. Этот атрибут является необязательным.  <br/> |
|Тип  <br/> |Указывает тип приложения.  <br/> |
|Область  <br/> |Область приложения.  <br/> |
|MarketplaceAssetId  <br/> |Указывает идентификатор средств marketplace приложения.  <br/> |
|MarketplaceContentMarket  <br/> |Определяет содержимое marketplace, пользователь видит для получения дополнительных сведений и дается обзор о приложении.  <br/> |
|AppStatus  <br/> |Указывает код состояния почтового приложения в непредвиденное состояние.  <br/> |
|Etoken  <br/> |Задает маркер лицензии платной или пробного почтовых приложений.  <br/> |
   
#### <a name="type"></a>Тип

|**Значение**|**Описание**|
|:-----|:-----|
|Значение по умолчанию  <br/> |Указывает, что приложение по умолчанию.  <br/> |
|частная переменная  <br/> |Указывает, что приложение является частной.  <br/> |
|Магазин  <br/> |Указывает, что приложение является приложением marketplace.  <br/> |
   
#### <a name="scope"></a>Область

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что приложение не будет иметь область.  <br/> |
|Пользователь  <br/> |Указывает, что приложение на одного пользователя.  <br/> |
|Организация  <br/> |Указывает, что приложение для организации.  <br/> |
|Значение по умолчанию  <br/> |Указывает, что приложение является стандартным приложением.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SpecificUsers](specificusers.md) <br/> |Задает учетных записей электронной почты, которые могут получить доступ к приложению.  <br/> |
|[Манифест](manifest.md) <br/> |Содержит файл манифеста приложения закодированный base-64.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |Указывает массив элементов **ClientExtension** .  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

