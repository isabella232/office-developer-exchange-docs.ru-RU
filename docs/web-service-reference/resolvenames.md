---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: Элемент ResolveNames определяет запрос на разрешение неоднозначных имен.
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467951"
---
# <a name="resolvenames"></a>ResolveNames

Элемент **ResolveNames** определяет запрос на разрешение неоднозначных имен. 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ресолвенаместипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ретурнфуллконтактдата** <br/> |Показывает, возвращаются ли в ответе полные контактные данные общедоступных контактов для общедоступного имени. Этот атрибут необходим для общедоступных контактов. Это значение не влияет на частные и частные списки рассылки, для которых идентификатор [ItemId](itemid.md) всегда возвращается.  <br/> |
|**SearchScope** <br/> |Определяет порядок и область поиска ResolveNames.  <br/> |
|контактдаташапе  <br/> |Определяет набор свойств, возвращаемый для контактов. Этот атрибут появился в Exchange Server 2010 с пакетом обновления 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Значения атрибутов Ретурнфуллконтактдата

|**Значение**|**Описание**|
|:-----|:-----|
|Верно.  <br/> |Возвращаются полные контактные данные для общедоступных контактов.  <br/> |
|False  <br/> |Полные контактные сведения для общедоступных контактов не возвращаются.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Значения атрибутов SearchScope

|**Значение**|**Описание**|
|:-----|:-----|
|ActiveDirectory  <br/> |Выполняется поиск только в службе каталогов Active Directory.  <br/> |
|активедиректориконтактс  <br/> |Сначала выполняется поиск в Active Directory, после чего выполняется поиск по папкам контактов, указанным в свойстве [парентфолдеридс](parentfolderids.md) .  <br/> |
|Контакты  <br/> |Выполняется поиск только папок контактов, определенных свойством [парентфолдеридс](parentfolderids.md) .  <br/> |
|контактсактиведиректори  <br/> |Папки контактов, идентифицируемые свойством [парентфолдеридс](parentfolderids.md) , сначала просматриваются, а затем в Active Directory выполняется поиск.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Значения атрибутов Контактдаташапе

|**Значение**|**Описание**|
|:-----|:-----|
|идонли  <br/> |Возвращается свойство идентификатора элемента Contact.  <br/> |
|По умолчанию  <br/> |Возвращается набор свойств элемента контакта по умолчанию. Дополнительные сведения о [фигурах ответа](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)см.  <br/> |
|аллпропертиес  <br/> |Возвращается набор Аллпропертиес для свойств элемента Contact. Дополнительные сведения о [фигурах ответа](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)см.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[парентфолдеридс](parentfolderids.md) <br/> |Содержит массив идентификаторов папок контактов, в которых будет выполняться поиск, если для атрибута **SearchScope** задано значение Активедиректориконтактс, Contacts или контактсактиведиректори. Массив Парентфолдеридс может содержать только один идентификатор папки контактов. Если элемент **парентфолдеридс** отсутствует, выполняется поиск по папке "Контакты" по умолчанию.  <br/> Идентификатор папки можно использовать для доступа к представителям.  <br/> Поиск в Active Directory выполняется с помощью списков управления доступом (ACL). У некоторых пользователей могут отсутствовать права на просмотр некоторых объектов Active Directory.  <br/> Этот элемент является необязательным.  <br/> |
|[унресолведентри](unresolvedentry.md) <br/> |Содержит имя контакта или списка рассылки, которые требуется разрешить.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

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



[Операция ResolveNames](resolvenames-operation.md)
  
[ресолвенаместипе](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ресолвенамессеарчскопетипе](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Использование разрешения имен](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

