---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: Элемент ClientExtension содержит сведения о пользователе и конфигурации приложения.
ms.openlocfilehash: fa02ad0f5f4312fefecee32d2ed24f0bb0585365
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519963"
---
# <a name="clientextension"></a>ClientExtension

Элемент **ClientExtension содержит** сведения о пользователе и конфигурации приложения. 
  
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
|IsAvailable  <br/> |Указывает, доступно ли приложение. Значение текста, **истинное** для **атрибута IsAvailable,** указывает на то, что приложение доступно. Значение false **указывает** на то, что приложение не доступно. Этот атрибут является необязательным.  <br/> |
|IsMandatory  <br/> |Указывает, является ли приложение обязательным. Значение **текста, истинное** для **атрибута IsMandatory,** указывает, что приложение является обязательным для почтового ящика. Значение false **указывает,** что приложение не является обязательным. Этот атрибут является необязательным.  <br/> |
|IsEnabledByDefault  <br/> |Указывает, включено ли приложение по умолчанию. Значение текста, **истинное для** **атрибута IsEnabledByDefault,** указывает на то, что приложение включено по умолчанию. Значение false **указывает,** что приложение не включено по умолчанию. Этот атрибут является необязательным.  <br/> |
|ProvidedTo  <br/> |Указывает, кому предоставлено приложение. Этот атрибут является необязательным.  <br/> |
|Type  <br/> |Указывает тип приложения.  <br/> |
|Область  <br/> |Указывает область приложения.  <br/> |
|MarketplaceAssetId  <br/> |Указывает идентификатор торгового актива приложения.  <br/> |
|MarketplaceContentMarket  <br/> |Указывает содержимое рынка, которое пользователь видит для подробных сведений и отзывов о приложении.  <br/> |
|AppStatus  <br/> |Указывает код состояния почтового приложения в неожиданном состоянии.  <br/> |
|Etoken  <br/> |Указывает маркер лицензии для платных или пробных почтовых приложений.  <br/> |
   
#### <a name="type"></a>Type

|**Значение**|**Описание**|
|:-----|:-----|
|По умолчанию  <br/> |Указывает, что приложение доступно по умолчанию.  <br/> |
|Закрытая  <br/> |Указывает, что приложение закрыто.  <br/> |
|MarketPlace  <br/> |Указывает, что приложение является приложением marketplace.  <br/> |
   
#### <a name="scope"></a>Область

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что приложение не имеет области.  <br/> |
|Пользователь  <br/> |Указывает, что приложение является для каждого пользователя.  <br/> |
|Организация  <br/> |Указывает, что приложение для организации.  <br/> |
|По умолчанию  <br/> |Указывает, что приложение является приложением по умолчанию.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SpecificUsers](specificusers.md) <br/> |Указывает учетные записи электронной почты, которые могут получить доступ к приложению.  <br/> |
|[Манифест](manifest.md) <br/> |Содержит кодированный файл манифеста приложения base-64.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |Указывает массив элементов **ClientExtension.**  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

