---
title: DelegateUsers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUsers
api_type:
- schema
ms.assetid: f30f80d9-20c8-41cc-afc7-a5eec1e0c5ea
description: Элемент DelegateUsers содержит идентификаторы делегатов для добавления или обновления в почтовом ящике. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: a078707ae6b1676ca5a32ba718add93debd498fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762010"
---
# <a name="delegateusers"></a><span data-ttu-id="69cd0-104">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="69cd0-104">DelegateUsers</span></span>

<span data-ttu-id="69cd0-105">Элемент **DelegateUsers** содержит идентификаторы делегатов для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="69cd0-105">The **DelegateUsers** element contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="69cd0-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="69cd0-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

<span data-ttu-id="69cd0-107">**ArrayOfDelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="69cd0-107">**ArrayOfDelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="69cd0-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="69cd0-108">Attributes and elements</span></span>

<span data-ttu-id="69cd0-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="69cd0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69cd0-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="69cd0-110">Attributes</span></span>

<span data-ttu-id="69cd0-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="69cd0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69cd0-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="69cd0-112">Child elements</span></span>

|<span data-ttu-id="69cd0-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69cd0-113">**Element**</span></span>|<span data-ttu-id="69cd0-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69cd0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69cd0-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="69cd0-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="69cd0-116">Определяет один делегат для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="69cd0-116">Identifies a single delegate to add to or update in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69cd0-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="69cd0-117">Parent elements</span></span>

|<span data-ttu-id="69cd0-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69cd0-118">**Element**</span></span>|<span data-ttu-id="69cd0-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69cd0-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69cd0-120">Метод AddDelegate</span><span class="sxs-lookup"><span data-stu-id="69cd0-120">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="69cd0-121">Определяет запрос на Добавление делегатов к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="69cd0-121">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="69cd0-122">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="69cd0-122">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="69cd0-123">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="69cd0-123">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="69cd0-124">Определяет запрос на обновление делегаты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="69cd0-124">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="69cd0-125">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="69cd0-125">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69cd0-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="69cd0-126">Remarks</span></span>

<span data-ttu-id="69cd0-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="69cd0-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69cd0-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="69cd0-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69cd0-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="69cd0-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69cd0-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="69cd0-130">Schema Name</span></span>  <br/> |<span data-ttu-id="69cd0-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="69cd0-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="69cd0-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="69cd0-132">Validation File</span></span>  <br/> |<span data-ttu-id="69cd0-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="69cd0-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69cd0-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="69cd0-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="69cd0-135">False</span><span class="sxs-lookup"><span data-stu-id="69cd0-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69cd0-136">См. также</span><span class="sxs-lookup"><span data-stu-id="69cd0-136">See also</span></span>

- [<span data-ttu-id="69cd0-137">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="69cd0-137">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="69cd0-138">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="69cd0-138">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="69cd0-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="69cd0-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="69cd0-140">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="69cd0-140">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

