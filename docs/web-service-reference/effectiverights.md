---
title: еффективеригхтс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: Элемент Еффективеригхтс содержит права клиента в зависимости от параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.
ms.openlocfilehash: 3055eb73056750508b48ead29136b56e7ce97ee9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459246"
---
# <a name="effectiverights"></a>еффективеригхтс

Элемент **еффективеригхтс** содержит права клиента в зависимости от параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 **еффективеригхтстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[креатеассоЦиатед](createassociated.md) <br/> |Указывает, может ли клиент создать связанную таблицу содержимого. Это свойство используется только для объектов Folder.  <br/> |
|[креатеконтентс](createcontents.md) <br/> |Указывает, может ли клиент создать таблицу содержимого. Это свойство используется только для объектов Folder.  <br/> |
|[креатехиерарчи](createhierarchy.md) <br/> |Указывает, может ли клиент создать таблицу иерархии. Это свойство используется только для объектов Folder.  <br/> |
|[Удаление](delete.md) <br/> |Указывает, может ли клиент удалить папку или элемент.  <br/> |
|[Modify](modify.md) <br/> |Указывает, может ли клиент изменить папку или элемент.  <br/> |
|[Read](read.md) <br/> |Указывает, может ли клиент прочитать папку или элемент.  <br/> |
|[виевприватеитемс](viewprivateitems.md) <br/> |Указывает, можно ли просматривать закрытый элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Представляет папку Tasks в почтовом ящике.  <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Представляет папку "Контакты" в почтовом ящике.  <br/> |
|[календарфолдер](calendarfolder.md) <br/> |Представляет папку "Календарь" в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Ресурс](item.md) <br/> |Представляет общий элемент Exchange.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент POST в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

**Еффективеригхтс** поддерживается в ответах на GetItem, GetItem, FindFolder, FindItem, SyncFolderHierarchy и SyncFolderItems. Свойство **еффективеригхтс** отображается в фигуре **аллпропертиес** для папок и элементов. 
  
Это свойство **еффективеригхтс** предоставляет доступ к тем же сведениям, что и в свойстве **MAPI PR_ACCESS** . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

