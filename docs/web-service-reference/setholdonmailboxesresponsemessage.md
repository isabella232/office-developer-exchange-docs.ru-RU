---
title: сесолдонмаилбоксесреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d61de0f3-24e0-434a-946a-c53d393b7d04
description: Элемент Сесолдонмаилбоксесреспонсемессаже указывает ответное сообщение для запроса SetHoldOnMailboxes.
ms.openlocfilehash: a6af4181218391bc9d3c177467295d771cce4c89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456411"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="9cc3b-103">сесолдонмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9cc3b-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="9cc3b-104">Элемент **сесолдонмаилбоксесреспонсемессаже** указывает ответное сообщение для запроса **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="9cc3b-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="9cc3b-105">**сесолдонмаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="9cc3b-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cc3b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9cc3b-106">Attributes and elements</span></span>

<span data-ttu-id="9cc3b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9cc3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cc3b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9cc3b-108">Attributes</span></span>

<span data-ttu-id="9cc3b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9cc3b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cc3b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9cc3b-110">Child elements</span></span>

<span data-ttu-id="9cc3b-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Маилбоксхолдресулт](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="9cc3b-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cc3b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9cc3b-112">Parent elements</span></span>

[<span data-ttu-id="9cc3b-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="9cc3b-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="9cc3b-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="9cc3b-114">Remarks</span></span>

<span data-ttu-id="9cc3b-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9cc3b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9cc3b-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9cc3b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cc3b-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9cc3b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cc3b-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9cc3b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9cc3b-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9cc3b-119">Schema name</span></span>  <br/> |<span data-ttu-id="9cc3b-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9cc3b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9cc3b-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9cc3b-121">Validation file</span></span>  <br/> |<span data-ttu-id="9cc3b-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9cc3b-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9cc3b-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9cc3b-123">Can be empty</span></span>  <br/> ||
   

