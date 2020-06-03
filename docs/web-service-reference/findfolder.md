---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: Элемент FindFolder определяет запрос на поиск папок в почтовом ящике.
ms.openlocfilehash: 248047206a661afe723543e52c51b57847148423
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462579"
---
# <a name="findfolder"></a>FindFolder

Элемент **FindFolder** определяет запрос на поиск папок в почтовом ящике. 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

**финдфолдертипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Обход  <br/> |Определяет способ выполнения поиска. Этот атрибут является обязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибутов обхода

|**Значение**|**Описание**|
|:-----|:-----|
|Поверхност  <br/> |Инструктирует операцию FindFolder для поиска только в идентифицированной папке и возврата только идентификаторов папок для элементов, которые не были удалены. Это называется неповерхностным обходом.  <br/> |
|Углублен  <br/> |Инструктирует операцию FindFolder для поиска во всех дочерних папках указанной родительской папки и возврата только идентификаторов папок для элементов, которые не были удалены. Это называется глубоким обходом.  <br/> |
|SoftDeleted  <br/> |Инструктирует операцию FindFolder для выполнения неполном обходного поиска для удаленных элементов.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдершапе](foldershape.md) <br/> |Определяет свойства папки, включаемые в отклике FindFolder.  <br/> |
|[индекседпажефолдервиев](indexedpagefolderview.md) <br/> |Описывает, как возвращаются сведения о страничном элементе в отклике FindFolder. Этот элемент является необязательным.  <br/> |
|[фрактионалпажефолдервиев](fractionalpagefolderview.md) <br/> |Описывает, где начинается страничное представление, и максимальное количество папок, возвращаемых в запросе FindFolder. Этот элемент является необязательным.  <br/> |
|[Restriction](restriction.md) <br/> |Определяет ограничение или запрос, используемый для фильтрации папок в операции FindFolder. Этот элемент является необязательным.  <br/> |
|[парентфолдеридс](parentfolderids.md) <br/> |Определяет папки для поиска в операции FindFolder.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере запроса FindFolder показано, как сформировать запрос на поиск всех папок, расположенных в папке "Входящие".
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindFolder](findfolder-operation.md)

