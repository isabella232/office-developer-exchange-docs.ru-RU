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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835420"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="f2d68-103">SetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f2d68-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="f2d68-104">Элемент **SetHoldOnMailboxesResponseMessage** указывает сообщение ответа на запрос **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="f2d68-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="f2d68-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f2d68-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2d68-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f2d68-106">Attributes and elements</span></span>

<span data-ttu-id="f2d68-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f2d68-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2d68-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f2d68-108">Attributes</span></span>

<span data-ttu-id="f2d68-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f2d68-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2d68-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f2d68-110">Child elements</span></span>

<span data-ttu-id="f2d68-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="f2d68-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2d68-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f2d68-112">Parent elements</span></span>

[<span data-ttu-id="f2d68-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f2d68-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="f2d68-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="f2d68-114">Remarks</span></span>

<span data-ttu-id="f2d68-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f2d68-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f2d68-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2d68-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2d68-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f2d68-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2d68-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f2d68-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f2d68-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f2d68-119">Schema name</span></span>  <br/> |<span data-ttu-id="f2d68-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f2d68-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f2d68-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f2d68-121">Validation file</span></span>  <br/> |<span data-ttu-id="f2d68-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f2d68-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f2d68-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f2d68-123">Can be empty</span></span>  <br/> ||
   

