---
title: Метод AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 646fb994-229e-4d90-8b95-6541191cb3ae
description: Элемент AddDelegate определяет запрос на Добавление делегатов к почтовому ящику. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d1cb0ff3ea68904bf88e346f68afe7c349ae4394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761342"
---
# <a name="adddelegate"></a><span data-ttu-id="16037-104">Метод AddDelegate</span><span class="sxs-lookup"><span data-stu-id="16037-104">AddDelegate</span></span>

<span data-ttu-id="16037-105">Элемент **AddDelegate** определяет запрос на Добавление делегатов к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="16037-105">The **AddDelegate** element defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="16037-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="16037-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<AddDelegate>
   <DelegateUsers/>
   <DeliverMeetingRequests/>
   <Mailbox/>
</AddDelegate>
```

 <span data-ttu-id="16037-107">**AddDelegateType**</span><span class="sxs-lookup"><span data-stu-id="16037-107">**AddDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16037-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="16037-108">Attributes and elements</span></span>

<span data-ttu-id="16037-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="16037-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16037-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="16037-110">Attributes</span></span>

<span data-ttu-id="16037-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="16037-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16037-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="16037-112">Child elements</span></span>

|<span data-ttu-id="16037-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16037-113">**Element**</span></span>|<span data-ttu-id="16037-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16037-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16037-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="16037-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="16037-116">Содержит идентификаторы делегатов для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="16037-116">Contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="16037-117">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="16037-117">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="16037-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="16037-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="16037-119">Определяет порядок обработки приглашений на собрания между делегата и участника.</span><span class="sxs-lookup"><span data-stu-id="16037-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="16037-120">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="16037-120">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="16037-121">Mailbox</span><span class="sxs-lookup"><span data-stu-id="16037-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="16037-122">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="16037-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="16037-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="16037-123">Parent elements</span></span>

<span data-ttu-id="16037-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="16037-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="16037-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="16037-125">Remarks</span></span>

<span data-ttu-id="16037-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="16037-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16037-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="16037-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16037-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="16037-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="16037-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="16037-129">Schema Name</span></span>  <br/> |<span data-ttu-id="16037-130">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="16037-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="16037-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="16037-131">Validation File</span></span>  <br/> |<span data-ttu-id="16037-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="16037-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="16037-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="16037-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="16037-134">False</span><span class="sxs-lookup"><span data-stu-id="16037-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16037-135">См. также</span><span class="sxs-lookup"><span data-stu-id="16037-135">See also</span></span>

- [<span data-ttu-id="16037-136">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="16037-136">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="16037-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="16037-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="16037-138">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="16037-138">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

