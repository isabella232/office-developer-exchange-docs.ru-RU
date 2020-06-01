---
title: унпинтеаммаилбокс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: Элемент Унпинтеаммаилбокс содержит запрос на открепление почтового ящика сайта от клиента путем его удаления из ответа автообнаружения.
ms.openlocfilehash: a6b01bfa9c5908765ff04ef7f5edbef0b99a9be2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467244"
---
# <a name="unpinteammailbox"></a><span data-ttu-id="2aea7-103">унпинтеаммаилбокс</span><span class="sxs-lookup"><span data-stu-id="2aea7-103">UnpinTeamMailbox</span></span>

<span data-ttu-id="2aea7-104">Элемент **унпинтеаммаилбокс** содержит запрос на открепление почтового ящика сайта от клиента путем его удаления из ответа **автообнаружения** .</span><span class="sxs-lookup"><span data-stu-id="2aea7-104">The **UnpinTeamMailbox** element contains the request to unpin a site mailbox from the client by removing it from the **Autodiscover** response.</span></span> 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 <span data-ttu-id="2aea7-105">**унпинтеаммаилбоксрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="2aea7-105">**UnpinTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2aea7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2aea7-106">Attributes and elements</span></span>

<span data-ttu-id="2aea7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2aea7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2aea7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2aea7-108">Attributes</span></span>

<span data-ttu-id="2aea7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2aea7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2aea7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2aea7-110">Child elements</span></span>

[<span data-ttu-id="2aea7-111">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2aea7-111">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="2aea7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2aea7-112">Parent elements</span></span>

<span data-ttu-id="2aea7-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="2aea7-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2aea7-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="2aea7-114">Remarks</span></span>

<span data-ttu-id="2aea7-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2aea7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2aea7-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2aea7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2aea7-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2aea7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2aea7-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2aea7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2aea7-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2aea7-119">Schema name</span></span>  <br/> |<span data-ttu-id="2aea7-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="2aea7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2aea7-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2aea7-121">Validation file</span></span>  <br/> |<span data-ttu-id="2aea7-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2aea7-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2aea7-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2aea7-123">Can be empty</span></span>  <br/> ||
   

