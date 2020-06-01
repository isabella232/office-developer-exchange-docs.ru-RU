---
title: сеарчмаилбоксесреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6f1bcbfb-d7f6-4fa0-b6f8-681a0b067007
description: Элемент Сеарчмаилбоксесреспонсемессаже указывает ответное сообщение для запроса SearchMailboxes.
ms.openlocfilehash: 342223b9a8cc7e91b97d637cb104f7bb160b7d5a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44448424"
---
# <a name="searchmailboxesresponsemessage"></a><span data-ttu-id="6c73e-103">сеарчмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6c73e-103">SearchMailboxesResponseMessage</span></span>

<span data-ttu-id="6c73e-104">Элемент **сеарчмаилбоксесреспонсемессаже** указывает ответное сообщение для запроса **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="6c73e-104">The **SearchMailboxesResponseMessage** element specifies the response message for a **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SearchMailboxesResult/>
</SearchMailboxesResponseMessage>
```

 <span data-ttu-id="6c73e-105">**сеарчмаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="6c73e-105">**SearchMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c73e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6c73e-106">Attributes and elements</span></span>

<span data-ttu-id="6c73e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6c73e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c73e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6c73e-108">Attributes</span></span>

<span data-ttu-id="6c73e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6c73e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c73e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6c73e-110">Child elements</span></span>

<span data-ttu-id="6c73e-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Сеарчмаилбоксесресулт](searchmailboxesresult.md)</span><span class="sxs-lookup"><span data-stu-id="6c73e-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchMailboxesResult](searchmailboxesresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c73e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6c73e-112">Parent elements</span></span>

<span data-ttu-id="6c73e-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6c73e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c73e-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="6c73e-114">Remarks</span></span>

<span data-ttu-id="6c73e-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6c73e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6c73e-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6c73e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c73e-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6c73e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c73e-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6c73e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c73e-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6c73e-119">Schema name</span></span>  <br/> |<span data-ttu-id="6c73e-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6c73e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c73e-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6c73e-121">Validation file</span></span>  <br/> |<span data-ttu-id="6c73e-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6c73e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c73e-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6c73e-123">Can be empty</span></span>  <br/> ||
   

