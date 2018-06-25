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
# <a name="lobbybypass"></a><span data-ttu-id="389e6-103">LobbyBypass</span><span class="sxs-lookup"><span data-stu-id="389e6-103">LobbyBypass</span></span>

<span data-ttu-id="389e6-104">Элемент **LobbyBypass** указывает на собрание по сети, установка для обхода виртуальный зал ожидания.</span><span class="sxs-lookup"><span data-stu-id="389e6-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="389e6-105">**LobbyBypassType**</span><span class="sxs-lookup"><span data-stu-id="389e6-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="389e6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="389e6-106">Attributes and elements</span></span>

<span data-ttu-id="389e6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="389e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="389e6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="389e6-108">Attributes</span></span>

<span data-ttu-id="389e6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="389e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="389e6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="389e6-110">Child elements</span></span>

<span data-ttu-id="389e6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="389e6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="389e6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="389e6-112">Parent elements</span></span>

[<span data-ttu-id="389e6-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="389e6-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="389e6-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="389e6-114">Text value</span></span>

<span data-ttu-id="389e6-115">Текстовое значение элемента **LobbyBypass** может быть **отключено** или **EnabledForGatewayParticipants**.</span><span class="sxs-lookup"><span data-stu-id="389e6-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="389e6-116">Значение **Этот параметр отключен** указывает, что обход зал ожидания отключен, поэтому необходимо доступ к всем участникам собрания с помощью виртуальных зал ожидания.</span><span class="sxs-lookup"><span data-stu-id="389e6-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="389e6-117">Значение **EnabledForGatewayParticipants** указывает, включено, что обход зал ожидания для участников телефона.</span><span class="sxs-lookup"><span data-stu-id="389e6-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="389e6-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="389e6-118">Remarks</span></span>

<span data-ttu-id="389e6-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="389e6-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="389e6-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="389e6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

