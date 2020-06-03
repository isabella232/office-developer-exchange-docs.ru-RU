---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: Элемент GetConversationItems определяет запрос на получение набора элементов, которые относятся к одной беседе.
ms.openlocfilehash: cde4bc2c39ccbc51b7436c87c4bc06e3b8d7e52c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457748"
---
# <a name="getconversationitems"></a><span data-ttu-id="4fa1a-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="4fa1a-103">GetConversationItems</span></span>

<span data-ttu-id="4fa1a-104">Элемент **GetConversationItems** определяет запрос на получение набора элементов, которые относятся к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="4fa1a-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
```XML
<GetConversationItems>
   <ItemShape/>
   <FoldersToIgnore/>
   <MaxItemsToReturn/>
   <SortOrder/>
   <MailboxScope/>
   <Conversations/>
</GetConversationItems>
```

 <span data-ttu-id="4fa1a-105">**жетконверсатионитемстипе**</span><span class="sxs-lookup"><span data-stu-id="4fa1a-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fa1a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4fa1a-106">Attributes and elements</span></span>

<span data-ttu-id="4fa1a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4fa1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fa1a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4fa1a-108">Attributes</span></span>

<span data-ttu-id="4fa1a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4fa1a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fa1a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4fa1a-110">Child elements</span></span>

<span data-ttu-id="4fa1a-111">[Итемшапе](itemshape.md)  |  [Фолдерстоигноре](folderstoignore.md)  |  [Макситемсторетурн](maxitemstoreturn.md)  |  [SortOrder (конверсатионнодесортордер)](sortorder-conversationnodesortorder.md)  |  [Маилбоксскопе](mailboxscope.md)  |  [Беседы](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="4fa1a-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fa1a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4fa1a-112">Parent elements</span></span>

<span data-ttu-id="4fa1a-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="4fa1a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4fa1a-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="4fa1a-114">Remarks</span></span>

<span data-ttu-id="4fa1a-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4fa1a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4fa1a-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fa1a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fa1a-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4fa1a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fa1a-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4fa1a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4fa1a-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4fa1a-119">Schema name</span></span>  <br/> |<span data-ttu-id="4fa1a-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4fa1a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4fa1a-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4fa1a-121">Validation file</span></span>  <br/> |<span data-ttu-id="4fa1a-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4fa1a-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4fa1a-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4fa1a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="4fa1a-124">false</span><span class="sxs-lookup"><span data-stu-id="4fa1a-124">false</span></span>  <br/> |
   

