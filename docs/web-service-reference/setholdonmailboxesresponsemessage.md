---
title: SetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d61de0f3-24e0-434a-946a-c53d393b7d04
description: Элемент SetHoldOnMailboxesResponseMessage указывает сообщение ответа на запрос SetHoldOnMailboxes.
ms.openlocfilehash: b7cb890a71d27340e328e39c1c463fefa080b8cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835420"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="55fc1-103">SetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="55fc1-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="55fc1-104">Элемент **SetHoldOnMailboxesResponseMessage** указывает сообщение ответа на запрос **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="55fc1-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="55fc1-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="55fc1-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55fc1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="55fc1-106">Attributes and elements</span></span>

<span data-ttu-id="55fc1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="55fc1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55fc1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="55fc1-108">Attributes</span></span>

<span data-ttu-id="55fc1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="55fc1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55fc1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="55fc1-110">Child elements</span></span>

<span data-ttu-id="55fc1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="55fc1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55fc1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="55fc1-112">Parent elements</span></span>

[<span data-ttu-id="55fc1-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="55fc1-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="55fc1-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="55fc1-114">Remarks</span></span>

<span data-ttu-id="55fc1-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="55fc1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="55fc1-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="55fc1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55fc1-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="55fc1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55fc1-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="55fc1-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55fc1-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="55fc1-119">Schema name</span></span>  <br/> |<span data-ttu-id="55fc1-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="55fc1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55fc1-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="55fc1-121">Validation file</span></span>  <br/> |<span data-ttu-id="55fc1-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="55fc1-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55fc1-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="55fc1-123">Can be empty</span></span>  <br/> ||
   

