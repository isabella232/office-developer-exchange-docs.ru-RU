---
title: жетнониндексаблеитемдетаилсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00566965-6cbd-4f31-9fa9-85b3e5559c0c
description: Элемент Жетнониндексаблеитемдетаилсреспонсемессаже указывает ответное сообщение для запроса GetNonIndexableItemDetails.
ms.openlocfilehash: 8df67294c17f9c9b786e73647878ad5b3586d788
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762855"
---
# <a name="getnonindexableitemdetailsresponsemessage"></a><span data-ttu-id="8c776-103">жетнониндексаблеитемдетаилсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="8c776-103">GetNonIndexableItemDetailsResponseMessage</span></span>

<span data-ttu-id="8c776-104">Элемент **жетнониндексаблеитемдетаилсреспонсемессаже** указывает ответное сообщение для запроса **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="8c776-104">The **GetNonIndexableItemDetailsResponseMessage** element specifies the response message for a **GetNonIndexableItemDetails** request.</span></span> 
  
```XML
<GetNonIndexableItemDetailsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponseMessage>
```

 <span data-ttu-id="8c776-105">**жетнониндексаблеитемдетаилсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8c776-105">**GetNonIndexableItemDetailsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c776-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8c776-106">Attributes and elements</span></span>

<span data-ttu-id="8c776-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8c776-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c776-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8c776-108">Attributes</span></span>

<span data-ttu-id="8c776-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8c776-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c776-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8c776-110">Child elements</span></span>

<span data-ttu-id="8c776-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md) [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md)дескриптивелинккэй мессажексмл нониндексаблеитемдетаилсресулт |  | </span><span class="sxs-lookup"><span data-stu-id="8c776-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8c776-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8c776-112">Parent elements</span></span>

[<span data-ttu-id="8c776-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="8c776-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="8c776-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="8c776-114">Remarks</span></span>

<span data-ttu-id="8c776-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8c776-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8c776-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c776-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c776-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8c776-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c776-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8c776-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8c776-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8c776-119">Schema name</span></span>  <br/> |<span data-ttu-id="8c776-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8c776-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8c776-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8c776-121">Validation file</span></span>  <br/> |<span data-ttu-id="8c776-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8c776-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8c776-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8c776-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8c776-124">false</span><span class="sxs-lookup"><span data-stu-id="8c776-124">false</span></span>  <br/> |
   

