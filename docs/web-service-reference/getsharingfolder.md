---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: Элемент GetSharingFolder определяет запрос на получение идентификатора локальной папки указанной общей папки. Это базовый элемент для операции GetSharingFolder.
ms.openlocfilehash: 7c2f31aa27c1cbde6cdad2b41a341916b4bed2ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833669"
---
# <a name="getsharingfolder"></a>GetSharingFolder

Элемент **GetSharingFolder** определяет запрос на получение идентификатора локальной папки указанной общей папки. Это базовый элемент для [операции GetSharingFolder](getsharingfolder-operation.md).
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **жетшарингфолдертипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Представляет SMTP-адрес электронной почты другой стороны в отношении совместного доступа. Этот элемент обязательный.  <br/> |
|[DataType](datatype.md) <br/> |Описывает тип данных, к которым предоставлен общий доступ в общей папке. Этот элемент является необязательным.  <br/> |
|[шаредфолдерид](sharedfolderid.md) <br/> |Представляет идентификатор общей папки, для которой должен быть возвращен идентификатор локальной папки. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Элемент GetSharingFolder должен содержать элемент [SmtpAddress](smtpaddress.md) . Элемент GetSharingFolder также должен содержать либо элемент [DataType](datatype.md) , либо элемент [шаредфолдерид](sharedfolderid.md) , но не может содержать и то, и другое. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingFolder](getsharingfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

