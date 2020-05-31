---
title: упдатеитеминрековераблеитемсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96259756-322e-4c24-ac76-0cd9c32e0d6d
description: Элемент Упдатеитеминрековераблеитемсреспонсемессаже указывает ответ на запрос Упдатеитеминрековераблеитемс.
ms.openlocfilehash: 598d91a4fbd4d241b75aea4c155caca68f120b3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840356"
---
# <a name="updateiteminrecoverableitemsresponsemessage"></a><span data-ttu-id="05110-103">упдатеитеминрековераблеитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="05110-103">UpdateItemInRecoverableItemsResponseMessage</span></span>

<span data-ttu-id="05110-104">Элемент **упдатеитеминрековераблеитемсреспонсемессаже** указывает ответ на запрос **упдатеитеминрековераблеитемс** .</span><span class="sxs-lookup"><span data-stu-id="05110-104">The **UpdateItemInRecoverableItemsResponseMessage** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKet/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponseMessage>
```

 <span data-ttu-id="05110-105">**упдатеитеминрековераблеитемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="05110-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05110-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="05110-106">Attributes and elements</span></span>

<span data-ttu-id="05110-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="05110-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05110-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="05110-108">Attributes</span></span>

<span data-ttu-id="05110-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="05110-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05110-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="05110-110">Child elements</span></span>

<span data-ttu-id="05110-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [MessageXml](messagexml.md)[Attachments](attachments-ex15websvcsotherref.md)[DescriptiveLinkKey](descriptivelinkkey.md) | [ConflictResults](conflictresults.md) [Items](items.md)дескриптивелинккэй мессажексмл | элементы | вложения конфликтресултс | </span><span class="sxs-lookup"><span data-stu-id="05110-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05110-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="05110-112">Parent elements</span></span>

<span data-ttu-id="05110-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="05110-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05110-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="05110-114">Remarks</span></span>

<span data-ttu-id="05110-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="05110-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="05110-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="05110-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05110-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="05110-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05110-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="05110-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="05110-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="05110-119">Schema name</span></span>  <br/> |<span data-ttu-id="05110-120">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="05110-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="05110-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="05110-121">Validation file</span></span>  <br/> |<span data-ttu-id="05110-122">Message. xsd</span><span class="sxs-lookup"><span data-stu-id="05110-122">Message.xsd</span></span>  <br/> |
|<span data-ttu-id="05110-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="05110-123">Can be empty</span></span>  <br/> |<span data-ttu-id="05110-124">false</span><span class="sxs-lookup"><span data-stu-id="05110-124">false</span></span>  <br/> |
   

