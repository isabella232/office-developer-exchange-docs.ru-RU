---
title: лоббибипасс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: Элемент Лоббибипасс указывает параметр собраний по сети, чтобы обойти виртуальный зал.
ms.openlocfilehash: 6940428c944b9d4d64acc6dbbf3993576e1932eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458098"
---
# <a name="lobbybypass"></a>лоббибипасс

Элемент **лоббибипасс** указывает параметр собраний по сети, чтобы обойти виртуальный зал. 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 **лоббибипасстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[онлинемитингсеттингс](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **лоббибипасс** может быть **отключено** или **енабледфоргатевайпартиЦипантс**. **Отключенное** значение указывает на то, что обход сервера-посредника отключен, поэтому все участники собрания должны получить доступ через виртуальный зал. Значение **енабледфоргатевайпартиЦипантс** указывает на то, что для участников в зале ожидания включена поддержка по телефону. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

