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
description: Элемент FindFolder определяет запрос для поиска папок в почтовом ящике.
ms.openlocfilehash: d41283547c443e38e2e87379a7224df9c89f901d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762559"
---
# <a name="findfolder"></a>FindFolder

Элемент **FindFolder** определяет запрос для поиска папок в почтовом ящике. 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

 **FindFolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Обход  <br/> |Определяет, как выполняется поиск. Этот атрибут является обязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибутов обхода

|**Значение**|**Описание**|
|:-----|:-----|
|Неполная  <br/> |Указывает, что операция FindFolder выполнять поиск только в указанной папке и для возвращения только в папке идентификаторов для элементов, которые не были удалены. Этот процесс называется частичного обхода.  <br/> |
|Глубокое  <br/> |Указывает, что операция FindFolder для поиска во всех дочерних папках определенного родительской папки и возвращает только в папке идентификаторов для элементов, которые не были удалены. Этот процесс называется глубину обхода.  <br/> |
|SoftDeleted  <br/> |Указывает, что операция FindFolder для выполнения поиска частичного обхода для удаленных элементов.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Задает свойства папки для включения в FindFolder ответа.  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |Описывает, как выгружаемый элемента сведения возвращаются в ответ FindFolder. Этот элемент является необязательным.  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |Описывает, где начала страничного представления и максимальное число папок, возвращаемых в запросе FindFolder. Этот элемент является необязательным.  <br/> |
|[Ограничения](restriction.md) <br/> |Задает ограничение или запрос, используемый для фильтрации папок в FindFolder операции. Этот элемент является необязательным.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Идентифицирует папок для операции FindFolder для поиска.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

Пример запроса FindFolder показано, как для формирования запроса, чтобы найти все папки, расположенной в папке "Входящие".
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindFolder Operation](findfolder-operation.md)

