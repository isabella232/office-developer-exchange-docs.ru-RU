---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: Элемент FractionalPageFolderView описывает, где начинается просмотр страницы и максимальное число папок, возвращающихся в запросе FindFolder.
ms.openlocfilehash: b3d4bd63f94c2db7761dabfad1e32558ceb30be5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530255"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

Элемент **FractionalPageFolderView** описывает, где начинается просмотр страницы и максимальное число папок, возвращающихся в [запросе FindFolder.](findfolder.md) 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Определяет максимальное количество результатов, возвращаемых в [ответе FindFolder.](findfolder.md) Этот атрибут является необязательным.  <br/> |
|**Числитель** <br/> |Представляет числитель дробного смещения с начала набора результатов. Этот атрибут является обязательным. Числитель должен быть равен или меньше, чем знаменатель. Этот атрибут должен представлять неотъемлемое значение, равное нулю или больше нуля. Дополнительные сведения см. в разделе Примечание в этой теме.  <br/> |
|**Знаменатель** <br/> |Представляет знаменатель дробного смещения с начала общего числа папок в наборе результатов. Этот атрибут является обязательным. Этот атрибут должен представлять неотъемлемое значение, которое больше одного. Дополнительные сведения см. в разделе Примечание в этой теме.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос на идентификацию папок в почтовом ящике.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Заметки

Смещение представления страницы с начала набора найденных папок описывается фракцией. Фракция, определяемая атрибутами **Numerator** и **Denominator,** описывает, где начинается страница информации. Например, если **Numerator** равен  четырем, а Знаменатель — пяти, страница возвращаемой информации начинается с записи, расположенной на четыре пятых пути к набору результатов. 
  
Если фракция оценивается до нуля, это указывает на начало набора результатов. Если фракция оценивается до одной, это указывает конец набора результатов.
  
> [!NOTE]
> Фракция представляет точки начала страницы, а не количество результатов в наборе результатов, которые будут возвращены. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindFolder](findfolder-operation.md)


[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

