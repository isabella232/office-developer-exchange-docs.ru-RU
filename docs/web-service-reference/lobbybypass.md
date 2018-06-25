---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: Элемент LobbyBypass указывает на собрание по сети, установка для обхода виртуальный зал ожидания.
ms.openlocfilehash: 9ecc920acd9e1aea3476ad1194d6c7d0529b21c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834246"
---
# <a name="lobbybypass"></a>LobbyBypass

Элемент **LobbyBypass** указывает на собрание по сети, установка для обхода виртуальный зал ожидания. 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 **LobbyBypassType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **LobbyBypass** может быть **отключено** или **EnabledForGatewayParticipants**. Значение **Этот параметр отключен** указывает, что обход зал ожидания отключен, поэтому необходимо доступ к всем участникам собрания с помощью виртуальных зал ожидания. Значение **EnabledForGatewayParticipants** указывает, включено, что обход зал ожидания для участников телефона. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

