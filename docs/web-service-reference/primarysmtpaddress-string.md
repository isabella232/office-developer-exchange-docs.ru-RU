---
title: Параметр PrimarySmtpAddress (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 706c6387-c648-4ccc-85e6-12a07b66da2f
description: Элемент PrimarySmtpAddress указывает основной адрес Simple Mail Transfer Protocol (SMTP) для почтового ящика.
ms.openlocfilehash: a103513c7cac94bd4923c12ed402b81c5d794e1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834878"
---
# <a name="primarysmtpaddress-string"></a><span data-ttu-id="6da1d-103">Параметр PrimarySmtpAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="6da1d-103">PrimarySmtpAddress (string)</span></span>

<span data-ttu-id="6da1d-104">Элемент **PrimarySmtpAddress** указывает основной адрес Simple Mail Transfer Protocol (SMTP) для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6da1d-104">The **PrimarySmtpAddress** element specifies the primary Simple Mail Transfer Protocol (SMTP) address of the mailbox.</span></span> 
  
```XML
<PrimarySmtpAddress></PrimarySmtpAddress>
```

 <span data-ttu-id="6da1d-105">**string**</span><span class="sxs-lookup"><span data-stu-id="6da1d-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6da1d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6da1d-106">Attributes and elements</span></span>

<span data-ttu-id="6da1d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6da1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6da1d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6da1d-108">Attributes</span></span>

<span data-ttu-id="6da1d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6da1d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6da1d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6da1d-110">Child elements</span></span>

<span data-ttu-id="6da1d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6da1d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6da1d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6da1d-112">Parent elements</span></span>

<span data-ttu-id="6da1d-113">[Идентификатор пользователя (string)](userid-string.md) | [почтового ящика (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [SearchableMailbox](searchablemailbox.md)</span><span class="sxs-lookup"><span data-stu-id="6da1d-113">[UserId (string)](userid-string.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [SearchableMailbox](searchablemailbox.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6da1d-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6da1d-114">Text value</span></span>

<span data-ttu-id="6da1d-115">Текстовое значение элемента **PrimarySmtpAddress** — это основной SMTP-адрес почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6da1d-115">The text value of the **PrimarySmtpAddress** element is the primary SMTP address of the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6da1d-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="6da1d-116">Remarks</span></span>

<span data-ttu-id="6da1d-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6da1d-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6da1d-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6da1d-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6da1d-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6da1d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6da1d-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6da1d-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6da1d-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6da1d-121">Schema name</span></span>  <br/> |<span data-ttu-id="6da1d-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6da1d-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="6da1d-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6da1d-123">Validation file</span></span>  <br/> |<span data-ttu-id="6da1d-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6da1d-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6da1d-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6da1d-125">Can be empty</span></span>  <br/> ||
   

