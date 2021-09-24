---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: Элемент GetSharingFolder определяет запрос для получения локального идентификатора папки указанной общей папки. Это базовый элемент для операции GetSharingFolder.
ms.openlocfilehash: 5d6362dff3ff29b0dc5100780cc70b21ec9bee9d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509772"
---
# <a name="getsharingfolder"></a>GetSharingFolder

Элемент **GetSharingFolder** определяет запрос для получения локального идентификатора папки указанной общей папки. Это базовый элемент для [операции GetSharingFolder.](getsharingfolder-operation.md)
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **GetSharingFolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Представляет адрес электронной почты SMTP другой стороны в отношениях общего доступа. Этот элемент обязательный.  <br/> |
|[DataType](datatype.md) <br/> |Описывает тип данных, общих для общей папки. Этот элемент является необязательным.  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |Представляет идентификатор общей папки, локальный идентификатор папки которой должен быть возвращен. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Элемент GetSharingFolder должен содержать [элемент SmtpAddress.](smtpaddress.md) Элемент GetSharingFolder также должен содержать элемент [DataType](datatype.md) или [элемент SharedFolderId,](sharedfolderid.md) но не может содержать оба элемента. 
  
Схема, описываемая этим элементом, расположена в виртуальном каталоге IIS, Exchange веб-службы компьютера, на котором Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingFolder](getsharingfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

