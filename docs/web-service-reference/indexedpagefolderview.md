---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: Элемент IndexedPageFolderView описывает, как сведения о странице возвращаются в ответе FindFolder.
ms.openlocfilehash: 0a5d0f7e63549b7a851862d957ff32dff4333ce3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542241"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

Элемент **IndexedPageFolderView** описывает, как сведения о странице возвращаются в [ответе FindFolder.](findfolder.md) 
  
[FindFolder](findfolder.md)
  
[IndexedPageFolderView](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Описывает максимальное количество папок, возвращающихся в ответ. Этот атрибут является необязательным.  <br/> |
|**Offset** <br/> |Описывает смещение из **BasePoint.** Смещение должно быть больше или равно нулю. Если **BasePoint** равен Началу, смещение является положительным. Если **BasePoint** равен End, смещение обрабатывается так, как если бы оно было отрицательным.  <br/> При этом определяется, какая папка будет первой папкой, доставленной в ответ. Этот атрибут является обязательным.  <br/> |
|**BasePoint** <br/> |Описывает, будет ли страница папок начинаться с самого начала или с конца набора папок, найденных с помощью критериев поиска. Поиск с конца всегда выполняет поиск в обратном направлении. Этот атрибут является обязательным.  <br/> |
   
#### <a name="basepoint-attribute"></a>Атрибут BasePoint

|**Значение**|**Описание**|
|:-----|:-----|
|Начало  <br/> |Просмотр страницы начинается в начале набора найденных папок.  <br/> |
|End  <br/> |Просмотр страницы начинается в конце набора найденных папок.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос на поиск папок в почтовом ящике.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Заметки

Поиск с конца включает перемещение в источник, идентифицированный смещением. Кроме того, указатель возвращается по количеству запрашиваемой записи. Например, если имеется 100 записей, а смещение — 25 с конца, поиск начинается с 75. Если возвращается 10 записей, указатель перемещается назад, дополнительные 10 записей — 65 и возвращает записи с 65 по 75. Следующий индекс — 64. Следующий смещение из конца страницы — 100 минус 64, что равно 36. Значение для следующего смещения из конца, чтобы получить следующую индексированную страницу 36.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

