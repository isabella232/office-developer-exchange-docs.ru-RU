---
title: UnpinTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: Элемент UnpinTeamMailbox содержит запрос, чтобы открепить почтового ящика сайта из клиента при удалении ответа службы автообнаружения.
ms.openlocfilehash: d303b47f0796f9bec7e9f198afa81d2ecd9fd5cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840295"
---
# <a name="unpinteammailbox"></a><span data-ttu-id="57787-103">UnpinTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="57787-103">UnpinTeamMailbox</span></span>

<span data-ttu-id="57787-104">Элемент **UnpinTeamMailbox** содержит запрос, чтобы открепить почтового ящика сайта из клиента при удалении ответа **службы автообнаружения** .</span><span class="sxs-lookup"><span data-stu-id="57787-104">The **UnpinTeamMailbox** element contains the request to unpin a site mailbox from the client by removing it from the **Autodiscover** response.</span></span> 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 <span data-ttu-id="57787-105">**UnpinTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="57787-105">**UnpinTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57787-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57787-106">Attributes and elements</span></span>

<span data-ttu-id="57787-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="57787-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57787-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57787-108">Attributes</span></span>

<span data-ttu-id="57787-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="57787-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57787-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57787-110">Child elements</span></span>

[<span data-ttu-id="57787-111">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="57787-111">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="57787-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57787-112">Parent elements</span></span>

<span data-ttu-id="57787-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="57787-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57787-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="57787-114">Remarks</span></span>

<span data-ttu-id="57787-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="57787-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57787-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="57787-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57787-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57787-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57787-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57787-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57787-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57787-119">Schema name</span></span>  <br/> |<span data-ttu-id="57787-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="57787-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57787-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57787-121">Validation file</span></span>  <br/> |<span data-ttu-id="57787-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="57787-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57787-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57787-123">Can be empty</span></span>  <br/> ||
   

