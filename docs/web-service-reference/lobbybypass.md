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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458098"
---
# <a name="lobbybypass"></a><span data-ttu-id="64e0c-103">лоббибипасс</span><span class="sxs-lookup"><span data-stu-id="64e0c-103">LobbyBypass</span></span>

<span data-ttu-id="64e0c-104">Элемент **лоббибипасс** указывает параметр собраний по сети, чтобы обойти виртуальный зал.</span><span class="sxs-lookup"><span data-stu-id="64e0c-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="64e0c-105">**лоббибипасстипе**</span><span class="sxs-lookup"><span data-stu-id="64e0c-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64e0c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64e0c-106">Attributes and elements</span></span>

<span data-ttu-id="64e0c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="64e0c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64e0c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64e0c-108">Attributes</span></span>

<span data-ttu-id="64e0c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="64e0c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64e0c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64e0c-110">Child elements</span></span>

<span data-ttu-id="64e0c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="64e0c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64e0c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64e0c-112">Parent elements</span></span>

[<span data-ttu-id="64e0c-113">онлинемитингсеттингс</span><span class="sxs-lookup"><span data-stu-id="64e0c-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="64e0c-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="64e0c-114">Text value</span></span>

<span data-ttu-id="64e0c-115">Текстовое значение элемента **лоббибипасс** может быть **отключено** или **енабледфоргатевайпартиЦипантс**.</span><span class="sxs-lookup"><span data-stu-id="64e0c-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="64e0c-116">**Отключенное** значение указывает на то, что обход сервера-посредника отключен, поэтому все участники собрания должны получить доступ через виртуальный зал.</span><span class="sxs-lookup"><span data-stu-id="64e0c-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="64e0c-117">Значение **енабледфоргатевайпартиЦипантс** указывает на то, что для участников в зале ожидания включена поддержка по телефону.</span><span class="sxs-lookup"><span data-stu-id="64e0c-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="64e0c-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="64e0c-118">Remarks</span></span>

<span data-ttu-id="64e0c-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="64e0c-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="64e0c-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="64e0c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

