---
title: Маркер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Token
api_type:
- schema
ms.assetid: 62b700e1-88c7-41ef-b431-d7af4a8b54a7
description: Элемент маркер содержит зашифрованные данные, который представляет маркер идентификации для общих данных.
ms.openlocfilehash: cec11d9f2c24a250483c5be6e273f981fdf0a8e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840209"
---
# <a name="token"></a>Маркер

**Маркер** элемент содержит зашифрованные данные, который представляет маркер идентификации для общих данных. 
  
```xml
<Token/>
```

 **EncryptedDataContainerType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EncryptedSharedFolderData](encryptedsharedfolderdata.md) <br/> |Содержит зашифрованные данные, которые клиент может использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

