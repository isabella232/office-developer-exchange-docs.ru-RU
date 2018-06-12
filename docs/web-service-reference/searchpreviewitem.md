---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: Элемент SearchPreviewItem указывает предварительного просмотра элемента для поиска обнаружения.
ms.openlocfilehash: 46b9d6049f856ce6e93b9e49e07516ec4b52d932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835308"
---
# <a name="searchpreviewitem"></a><span data-ttu-id="91039-103">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="91039-103">SearchPreviewItem</span></span>

<span data-ttu-id="91039-104">Элемент **SearchPreviewItem** указывает предварительного просмотра элемента для поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="91039-104">The **SearchPreviewItem** element specifies the item preview for a discovery search.</span></span> 
  
```XML
<SearchPreviewItem>
   <Id/>
   <Mailbox/>
   <ParentId/>
   <ItemClass/>
   <UniqueHash/>
   <SortValue/>
   <OwaLink/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <CreatedTime/>
   <ReceivedTime/>
   <SentTime/>
   <Subject/>
   <Size/>
   <Preview/>
   <Importance/>
   <Read/>
   <HasAttachment/>
   <ExtendedProperties/>
</SearchPreviewItem>
```

 <span data-ttu-id="91039-105">**SearchPreviewItemType**</span><span class="sxs-lookup"><span data-stu-id="91039-105">**SearchPreviewItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91039-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="91039-106">Attributes and elements</span></span>

<span data-ttu-id="91039-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="91039-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91039-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="91039-108">Attributes</span></span>

<span data-ttu-id="91039-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="91039-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91039-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="91039-110">Child elements</span></span>

<span data-ttu-id="91039-111">[Идентификатор (ItemIdType)](id-itemidtype.md) | [почтового ящика (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md)  |  [ Отправитель (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md)  |  [SentTime](senttime.md)  |  [Темы](subject.md) | [размер (длинный)](size-long.md) | [предварительной версии](preview-ex15websvcsotherref.md) | [Важность](importance.md) | [чтения](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties () NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span><span class="sxs-lookup"><span data-stu-id="91039-111">[ID (ItemIdType)](id-itemidtype.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md) | [Sender (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [Subject](subject.md) | [Size (long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [Read](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91039-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="91039-112">Parent elements</span></span>

[<span data-ttu-id="91039-113">Элементы (ArrayOfSearchPreviewItemsType)</span><span class="sxs-lookup"><span data-stu-id="91039-113">Items (ArrayOfSearchPreviewItemsType)</span></span>](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a><span data-ttu-id="91039-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="91039-114">Remarks</span></span>

<span data-ttu-id="91039-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="91039-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91039-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="91039-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91039-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="91039-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91039-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="91039-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91039-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="91039-119">Schema name</span></span>  <br/> |<span data-ttu-id="91039-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="91039-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="91039-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="91039-121">Validation file</span></span>  <br/> |<span data-ttu-id="91039-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91039-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91039-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="91039-123">Can be empty</span></span>  <br/> ||
   

