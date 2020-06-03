---
title: енкриптедшаредфолдердата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: Элемент Енкриптедшаредфолдердата содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.
ms.openlocfilehash: 52e91eaf1ded31602b11e50c1b62159f72c101cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530665"
---
# <a name="encryptedsharedfolderdata"></a>енкриптедшаредфолдердата

Элемент **енкриптедшаредфолдердата** содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами. 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 **енкриптедшаредфолдердататипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Маркер](token.md) <br/> |Содержит зашифрованные данные, представляющие маркер идентификации для общих данных.  <br/> |
|[Data](data.md) <br/> |Содержит зашифрованные данные, представляющие общие данные.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[енкриптедшаредфолдердатаколлектион](encryptedsharedfolderdatacollection.md) <br/> |Представляет коллекцию структур данных, которую клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetSharingMetadata](getsharingmetadata-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

