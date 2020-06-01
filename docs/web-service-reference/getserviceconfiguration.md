---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: Элемент GetServiceConfiguration определяет запрос GetServiceConfiguration.
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457874"
---
# <a name="getserviceconfiguration"></a>GetServiceConfiguration

Элемент **GetServiceConfiguration** определяет запрос GetServiceConfiguration. 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 **жетсервицеконфигуратионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[актингас](actingas.md) <br/> |Указывает, кому отправляется вызывающий абонент. Этот элемент является необязательным. Если этот элемент отсутствует, предполагается, что пользователь, прошедший проверку подлинности, является отправителем. Элемент **актингас** должен быть включен для запроса подсказок отправителя. Если элемент **актингас** отсутствует, в отклике может быть возвращена ошибка ерроринвалидаргумент, не включающая в себя тип маршрутизации, не включает адрес электронной почты, содержит недопустимый адрес электронной почты, не разрешается пользователю в доменных службах Active Directory (AD DS) или разрешается нескольким пользователям в доменных службах Active Directory.  <br/> |
|[рекуестедконфигуратион](requestedconfiguration.md) <br/> |Содержит требуемые конфигурации службы. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
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

