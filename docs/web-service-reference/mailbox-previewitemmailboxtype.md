---
title: Почтовый ящик (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: Элемент почтовых ящиков содержит идентификатор почтового ящика и основной адрес Simple Mail Transfer Protocol (SMTP).
ms.openlocfilehash: 1b6669928015bc880806479d294a4063034a559f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834255"
---
# <a name="mailbox-previewitemmailboxtype"></a><span data-ttu-id="db831-103">Почтовый ящик (PreviewItemMailboxType)</span><span class="sxs-lookup"><span data-stu-id="db831-103">Mailbox (PreviewItemMailboxType)</span></span>

<span data-ttu-id="db831-104">Элемент **почтовых ящиков** содержит идентификатор почтового ящика и основной адрес Simple Mail Transfer Protocol (SMTP).</span><span class="sxs-lookup"><span data-stu-id="db831-104">The **Mailbox** element contains the mailbox identifier and the user's primary Simple Mail Transfer Protocol (SMTP) address.</span></span> 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

<span data-ttu-id="db831-105">**PreviewItemMailboxType**</span><span class="sxs-lookup"><span data-stu-id="db831-105">**PreviewItemMailboxType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="db831-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db831-106">Attributes and elements</span></span>

<span data-ttu-id="db831-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="db831-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db831-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db831-108">Attributes</span></span>

<span data-ttu-id="db831-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="db831-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db831-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db831-110">Child elements</span></span>

<span data-ttu-id="db831-111">[MailboxId](mailboxid.md) | [PrimarySmtpAddress (строка)](primarysmtpaddress-string.md)</span><span class="sxs-lookup"><span data-stu-id="db831-111">[MailboxId](mailboxid.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db831-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db831-112">Parent elements</span></span>

[<span data-ttu-id="db831-113">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="db831-113">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="db831-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="db831-114">Remarks</span></span>

<span data-ttu-id="db831-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="db831-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="db831-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="db831-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db831-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db831-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db831-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db831-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db831-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db831-119">Schema name</span></span>  <br/> |<span data-ttu-id="db831-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="db831-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="db831-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db831-121">Validation file</span></span>  <br/> |<span data-ttu-id="db831-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="db831-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db831-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db831-123">Can be empty</span></span>  <br/> |<span data-ttu-id="db831-124">Нет</span><span class="sxs-lookup"><span data-stu-id="db831-124">false</span></span>  <br/> |
   

