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
ms.openlocfilehash: e0eb1fbd7155040508daf253f5eb4b1352d7426d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835485"
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

Нет.
  
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

