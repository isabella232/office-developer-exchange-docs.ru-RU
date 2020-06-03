---
title: жетаппманифестсреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: Элемент Жетаппманифестсреспонсе определяет ответ на запрос операции GetAppManifests.
ms.openlocfilehash: a01f6265d6d534e2f7868b17acf19f0f5d52a01f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462966"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="6ef5d-103">жетаппманифестсреспонсе</span><span class="sxs-lookup"><span data-stu-id="6ef5d-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="6ef5d-104">Элемент **жетаппманифестсреспонсе** определяет ответ на запрос операции **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="6ef5d-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Manifests/>
</GetAppManifestsResponse>
```

```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Apps/>
</GetAppManifestsResponse>
```

<span data-ttu-id="6ef5d-105">**жетаппманифестсреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="6ef5d-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6ef5d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6ef5d-106">Attributes and elements</span></span>

<span data-ttu-id="6ef5d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6ef5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ef5d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6ef5d-108">Attributes</span></span>

<span data-ttu-id="6ef5d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6ef5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ef5d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6ef5d-110">Child elements</span></span>

<span data-ttu-id="6ef5d-111">[Респонсекоде](responsecode.md)  |  [Манифесты](manifests.md)  |  [Приложения](apps.md)</span><span class="sxs-lookup"><span data-stu-id="6ef5d-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ef5d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6ef5d-112">Parent elements</span></span>

<span data-ttu-id="6ef5d-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6ef5d-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ef5d-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="6ef5d-114">Remarks</span></span>

<span data-ttu-id="6ef5d-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6ef5d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6ef5d-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ef5d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ef5d-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6ef5d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ef5d-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6ef5d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6ef5d-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6ef5d-119">Schema Name</span></span>  <br/> |<span data-ttu-id="6ef5d-120">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="6ef5d-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="6ef5d-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6ef5d-121">Validation File</span></span>  <br/> |<span data-ttu-id="6ef5d-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6ef5d-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ef5d-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6ef5d-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="6ef5d-124">False</span><span class="sxs-lookup"><span data-stu-id="6ef5d-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ef5d-125">См. также</span><span class="sxs-lookup"><span data-stu-id="6ef5d-125">See also</span></span>

- [<span data-ttu-id="6ef5d-126">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6ef5d-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

