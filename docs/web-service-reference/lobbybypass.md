---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: Элемент LobbyBypass указывает параметр собрания в Интернете для обхода виртуального вестибюля.
ms.openlocfilehash: 41ab9c3f846112d2b679bbb477a0de355a477ffa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540785"
---
# <a name="lobbybypass"></a>LobbyBypass

Элемент **LobbyBypass** указывает параметр собрания в Интернете для обхода виртуального вестибюля. 
  
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

Текстовое значение элемента **LobbyBypass** может  быть отключено или **включеноForGatewayParticipants.** Значение **Отключено** указывает, что обход вестибюля отключен, поэтому всем участникам собрания необходимо получить доступ через виртуальное лобби. Значение **EnabledForGatewayParticipants** указывает, что для участников телефонной связи включен обход вестибюля. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

