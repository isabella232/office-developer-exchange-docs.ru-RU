---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: Элемент GetSharingMetadata определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию. Этот элемент является базовым элементом для операции GetSharingMetadata.
ms.openlocfilehash: 5283d35e11350ef10ed8cc01527e787ef54be927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833677"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

Элемент **GetSharingMetadata** определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию. Этот элемент является базовым элементом для [операции GetSharingMetadata](getsharingmetadata-operation.md).
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 **жетшарингметадататипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[идоффолдертошаре](idoffoldertoshare.md) <br/> |Представляет идентификатор папки на сервере, к которой будет предоставлен общий доступ. Этот элемент обязательный.  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |Представляет SMTP-адрес электронной почты, соответствующий почтовому ящику, содержащему папку, определяемую элементом [идоффолдертошаре](idoffoldertoshare.md) . Этот элемент обязательный.  <br/> |
|[Получатели (Аррайофсмтпаддресстипе)](recipients-arrayofsmtpaddresstype.md) <br/> |Представляет SMTP-адреса электронной почты одного или нескольких сущностей, которым будет предоставлен доступ к данным в папке, указанной с помощью элемента [идоффолдертошаре](idoffoldertoshare.md) . Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

