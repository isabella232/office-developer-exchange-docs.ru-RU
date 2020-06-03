---
title: ексчанжеимперсонатион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: Элемент Ексчанжеимперсонатион используется в заголовке SOAP запроса. Когда этот элемент присутствует, вызывающий абонент пытается олицетворить учетную запись, содержащуюся в элементе Ексчанжеимперсонатион.
ms.openlocfilehash: 188219d95453dc45378c6ca65ab93c2de7db4eac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463351"
---
# <a name="exchangeimpersonation"></a>ексчанжеимперсонатион

Элемент **ексчанжеимперсонатион** используется в заголовке SOAP запроса. Когда этот элемент присутствует, вызывающий абонент пытается олицетворить учетную запись, содержащуюся в элементе **ексчанжеимперсонатион** . 
  
[ексчанжеимперсонатион](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 **ексчанжеимперсонатионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[коннектингсид](connectingsid.md) <br/> |Представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Вызывающая учетная запись должна иметь **MS-дов-олицетворение** прямо на сервере клиентского доступа и в службе **MS-дов-майимперсонате** в базе данных почтовых ящиков, которая содержит почтовый ящик для олицетворения или объекта пользователя или контакта Active Directory. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Авторизация между серверами в EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

