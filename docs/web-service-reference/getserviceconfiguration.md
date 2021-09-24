---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: Элемент GetServiceConfiguration определяет запрос GetServiceConfiguration.
ms.openlocfilehash: fdc4fd84c658dd0cd2ecabe7fefc06113bca173a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533436"
---
# <a name="getserviceconfiguration"></a>GetServiceConfiguration

Элемент **GetServiceConfiguration** определяет запрос GetServiceConfiguration. 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 **GetServiceConfigurationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Определяет, кому отправляется вызываемая. Этот элемент является необязательным. Если этого элемента нет, предполагается, что отправительом является пользователь, заверяемый в проверке подлинности. Элемент **ActingAs** должен быть включен для запроса подсказки отправитель. Ошибка ErrorInvalidArgument может быть возвращена в ответ, если элемент **ActingAs** отсутствует, не включает тип маршрутизирования, не включает адрес электронной почты, содержит недействительный адрес электронной почты, не устраняет пользователя в службе доменных служб Active Directory (AD DS) или решает для нескольких пользователей в AD DS.  <br/> |
|[RequestedConfiguration](requestedconfiguration.md) <br/> |Содержит запрашиваемую конфигурацию службы. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
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

