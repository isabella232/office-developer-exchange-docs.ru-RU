---
title: UpdateItemInRecoverableItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2f61b038-eba0-40fc-8af2-c3db5cc5a420
description: Элемент UpdateItemInRecoverableItemsResponse указывает ответ на запрос UpdateItemInRecoverableItems.
ms.openlocfilehash: 2cb9bcb2752599a546c1391d6ea306735b3b0c78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840354"
---
# <a name="updateiteminrecoverableitemsresponse"></a><span data-ttu-id="ebbe1-103">UpdateItemInRecoverableItemsResponse</span><span class="sxs-lookup"><span data-stu-id="ebbe1-103">UpdateItemInRecoverableItemsResponse</span></span>

<span data-ttu-id="ebbe1-104">Элемент **UpdateItemInRecoverableItemsResponse** указывает ответ на запрос **UpdateItemInRecoverableItems** .</span><span class="sxs-lookup"><span data-stu-id="ebbe1-104">The **UpdateItemInRecoverableItemsResponse** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponse>
```

 <span data-ttu-id="ebbe1-105">**UpdateItemInRecoverableItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ebbe1-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebbe1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ebbe1-106">Attributes and elements</span></span>

<span data-ttu-id="ebbe1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ebbe1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebbe1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ebbe1-108">Attributes</span></span>

<span data-ttu-id="ebbe1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ebbe1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebbe1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ebbe1-110">Child elements</span></span>

<span data-ttu-id="ebbe1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [элементы](items.md) | [вложения](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="ebbe1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ebbe1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ebbe1-112">Parent elements</span></span>

<span data-ttu-id="ebbe1-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="ebbe1-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ebbe1-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="ebbe1-114">Remarks</span></span>

<span data-ttu-id="ebbe1-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ebbe1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ebbe1-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ebbe1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebbe1-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ebbe1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebbe1-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ebbe1-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ebbe1-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ebbe1-119">Schema name</span></span>  <br/> |<span data-ttu-id="ebbe1-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ebbe1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ebbe1-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ebbe1-121">Validation file</span></span>  <br/> |<span data-ttu-id="ebbe1-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ebbe1-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ebbe1-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ebbe1-123">Can be empty</span></span>  <br/> |<span data-ttu-id="ebbe1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ebbe1-124">false</span></span>  <br/> |
   

