---
title: сеарчаблемаилбокс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: Элемент Сеарчаблемаилбокс указывает почтовый ящик, возвращенный из запроса GetSearchableMailboxes.
ms.openlocfilehash: f790d9a707f10f64a776b2fc35255c233ad854b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467454"
---
# <a name="searchablemailbox"></a><span data-ttu-id="8b0ab-103">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="8b0ab-103">SearchableMailbox</span></span>

<span data-ttu-id="8b0ab-104">Элемент **сеарчаблемаилбокс** указывает почтовый ящик, возвращенный из запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="8b0ab-104">The **SearchableMailbox** element specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 <span data-ttu-id="8b0ab-105">**сеарчаблемаилбокстипе**</span><span class="sxs-lookup"><span data-stu-id="8b0ab-105">**SearchableMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b0ab-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b0ab-106">Attributes and elements</span></span>

<span data-ttu-id="8b0ab-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8b0ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b0ab-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b0ab-108">Attributes</span></span>

<span data-ttu-id="8b0ab-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8b0ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b0ab-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b0ab-110">Child elements</span></span>

<span data-ttu-id="8b0ab-111">[Идентификатор GUID](guid-ex15websvcsotherref.md)  |  [PrimarySmtpAddress (строка)](primarysmtpaddress-string.md)  |  [Исекстерналмаилбокс](isexternalmailbox.md)  |  [ExternalEmailAddress](externalemailaddress.md)  |  [DisplayName (строка)](displayname-string.md)  |  [Исмембершипграуп](ismembershipgroup.md)  |  [Референцеид](referenceid.md)</span><span class="sxs-lookup"><span data-stu-id="8b0ab-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md) | [ReferenceId](referenceid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b0ab-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b0ab-112">Parent elements</span></span>

[<span data-ttu-id="8b0ab-113">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="8b0ab-113">SearchableMailboxes</span></span>](searchablemailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="8b0ab-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="8b0ab-114">Remarks</span></span>

<span data-ttu-id="8b0ab-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8b0ab-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8b0ab-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b0ab-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b0ab-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b0ab-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b0ab-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b0ab-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b0ab-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b0ab-119">Schema name</span></span>  <br/> |<span data-ttu-id="8b0ab-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8b0ab-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b0ab-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b0ab-121">Validation file</span></span>  <br/> |<span data-ttu-id="8b0ab-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8b0ab-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b0ab-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b0ab-123">Can be empty</span></span>  <br/> ||
   

