---
title: шарингфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: Элемент Шарингфолдерид представляет идентификатор локальной папки в отношении общего доступа.
ms.openlocfilehash: 02780251639ee651ca65d8eadded43260852aaf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526580"
---
# <a name="sharingfolderid"></a>шарингфолдерид

Элемент **шарингфолдерид** представляет идентификатор локальной папки в отношении общего доступа. 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 **фолдеридтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Содержит строку, определяющую папку в хранилище Exchange. Этот атрибут является обязательным.  <br/> |
|чанжекэй  <br/> |Содержит строку, определяющую версию папки, определяемую атрибутом ID. Этот атрибут является необязательным. Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RefreshSharingFolder](refreshsharingfolder.md) <br/> |Определяет запрос на обновление указанной локальной папки.  <br/> |
|[жетшарингфолдерреспонсе](getsharingfolderresponse.md) <br/> |Определяет ответ на запрос [операции GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[жетшарингфолдерреспонсемессаже](getsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

