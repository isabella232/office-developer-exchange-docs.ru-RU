---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: Элемент FindFolder определяет запрос на поиск папок в почтовом ящике.
ms.openlocfilehash: 431efde28e417efec04f6fa1625a81b3766cb705
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518444"
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

**FindFolderType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Traversal  <br/> |Определяет, как выполняется поиск. Этот атрибут является обязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибута Traversal

|**Значение**|**Описание**|
|:-----|:-----|
|Shallow  <br/> |Предписывает операции FindFolder искать только выявленную папку и возвращать только те папки, которые не были удалены. Это называется неглубоким обходом.  <br/> |
|Deep  <br/> |Предписывает операции FindFolder искать во всех детских папках идентифицированной родительской папки и возвращать только те папки, которые не были удалены. Это называется глубоким обходом.  <br/> |
|SoftDeleted  <br/> |Инструктаже операции FindFolder для выполнения неглубокого обходного поиска удаленных элементов.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Определяет свойства папки, которые необходимо включить в ответ FindFolder.  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |Описывает, как возвращаются сведения о странице в ответе FindFolder. Этот элемент является необязательным.  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |Описывает, где начинается просмотр страницы и максимальное число папок, возвращающихся в запросе FindFolder. Этот элемент является необязательным.  <br/> |
|[Restriction](restriction.md) <br/> |Определяет ограничение или запрос, используемый для фильтрации папок в операции FindFolder. Этот элемент является необязательным.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Определяет папки для операции FindFolder для поиска.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере запроса FindFolder показано, как сформировать запрос, чтобы найти все папки, расположенные в папке "Входящие".
  
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
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindFolder](findfolder-operation.md)

