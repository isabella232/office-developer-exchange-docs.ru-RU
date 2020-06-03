---
title: делегатеусерс
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
description: Элемент Делегатеусерс содержит идентификаторы делегатов, которые добавляются в почтовый ящик или обновляются в нем. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 69f5aab65634f41ec0f820da05dee79a300fb32e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457377"
---
# <a name="delegateusers"></a><span data-ttu-id="eac0e-104">делегатеусерс</span><span class="sxs-lookup"><span data-stu-id="eac0e-104">DelegateUsers</span></span>

<span data-ttu-id="eac0e-105">Элемент **делегатеусерс** содержит идентификаторы делегатов, которые добавляются в почтовый ящик или обновляются в нем.</span><span class="sxs-lookup"><span data-stu-id="eac0e-105">The **DelegateUsers** element contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="eac0e-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="eac0e-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

<span data-ttu-id="eac0e-107">**аррайофделегатеусертипе**</span><span class="sxs-lookup"><span data-stu-id="eac0e-107">**ArrayOfDelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="eac0e-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eac0e-108">Attributes and elements</span></span>

<span data-ttu-id="eac0e-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="eac0e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eac0e-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eac0e-110">Attributes</span></span>

<span data-ttu-id="eac0e-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="eac0e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eac0e-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eac0e-112">Child elements</span></span>

|<span data-ttu-id="eac0e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eac0e-113">**Element**</span></span>|<span data-ttu-id="eac0e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eac0e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eac0e-115">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="eac0e-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="eac0e-116">Определяет одного делегата для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="eac0e-116">Identifies a single delegate to add to or update in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eac0e-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eac0e-117">Parent elements</span></span>

|<span data-ttu-id="eac0e-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eac0e-118">**Element**</span></span>|<span data-ttu-id="eac0e-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eac0e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eac0e-120">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="eac0e-120">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="eac0e-121">Определяет запрос на добавление делегатов в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="eac0e-121">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="eac0e-122">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="eac0e-122">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="eac0e-123">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="eac0e-123">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="eac0e-124">Определяет запрос на обновление делегатов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="eac0e-124">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="eac0e-125">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="eac0e-125">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eac0e-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="eac0e-126">Remarks</span></span>

<span data-ttu-id="eac0e-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="eac0e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eac0e-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eac0e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eac0e-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eac0e-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eac0e-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eac0e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="eac0e-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="eac0e-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="eac0e-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eac0e-132">Validation File</span></span>  <br/> |<span data-ttu-id="eac0e-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="eac0e-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eac0e-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eac0e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="eac0e-135">False</span><span class="sxs-lookup"><span data-stu-id="eac0e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eac0e-136">См. также</span><span class="sxs-lookup"><span data-stu-id="eac0e-136">See also</span></span>

- [<span data-ttu-id="eac0e-137">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="eac0e-137">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="eac0e-138">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="eac0e-138">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="eac0e-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="eac0e-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="eac0e-140">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="eac0e-140">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

