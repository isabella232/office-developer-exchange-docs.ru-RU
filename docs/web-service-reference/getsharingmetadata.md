---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: Элемент GetSharingMetadata определяет запрос на получения непрозрачного маркера проверки подлинности, который идентифицирует приглашение к совместному доступу. Этот элемент является базовым элементом для операции GetSharingMetadata.
ms.openlocfilehash: 65da8371b25c42e59f898c79403f06fa17e5a24a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523056"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

Элемент **GetSharingMetadata** определяет запрос на получения непрозрачного маркера проверки подлинности, который идентифицирует приглашение к совместному доступу. Этот элемент является базовым элементом для [операции GetSharingMetadata.](getsharingmetadata-operation.md)
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 **GetSharingMetadataType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[IdOfFolderToShare](idoffoldertoshare.md) <br/> |Представляет идентификатор папки на сервере, который будет общим. Этот элемент обязательный.  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |Представляет адрес электронной почты SMTP, соответствующий почтовому ящику, который содержит папку, идентифицированную элементом [IdOfFolderToShare.](idoffoldertoshare.md) Этот элемент обязательный.  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Представляет адреса электронной почты SMTP одного или более сущностям, которые будут предоставлены доступ к данным в папке, идентифицированной элементом [IdOfFolderToShare.](idoffoldertoshare.md) Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

