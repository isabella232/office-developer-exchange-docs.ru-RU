---
title: RemoveDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: f21c5171-62e7-47c8-99b1-22e1ff5883bb
description: Элемент RemoveDelegate определяет запрос для удаления делегатов из почтового ящика. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 27618b1767c99b26a5f4c06e97a20e063b598d9d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835085"
---
# <a name="removedelegate"></a><span data-ttu-id="29432-104">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="29432-104">RemoveDelegate</span></span>

<span data-ttu-id="29432-105">Элемент **RemoveDelegate** определяет запрос для удаления делегатов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="29432-105">The **RemoveDelegate** element defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="29432-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="29432-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<RemoveDelegate>
      <Mailbox/>
   <UserIds/>
</RemoveDelegate>
```

 <span data-ttu-id="29432-107">**RemoveDelegateType**</span><span class="sxs-lookup"><span data-stu-id="29432-107">**RemoveDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29432-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="29432-108">Attributes and elements</span></span>

<span data-ttu-id="29432-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="29432-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29432-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="29432-110">Attributes</span></span>

<span data-ttu-id="29432-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="29432-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29432-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="29432-112">Child elements</span></span>

|<span data-ttu-id="29432-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="29432-113">**Element**</span></span>|<span data-ttu-id="29432-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="29432-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29432-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="29432-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="29432-116">Определяет основного сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="29432-116">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="29432-117">UserIds</span><span class="sxs-lookup"><span data-stu-id="29432-117">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="29432-118">Содержит массив делегат пользователям удалять из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="29432-118">Contains an array of delegate users to remove from a principal's mailbox.</span></span> <span data-ttu-id="29432-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="29432-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29432-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="29432-120">Parent elements</span></span>

<span data-ttu-id="29432-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="29432-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="29432-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="29432-122">Remarks</span></span>

<span data-ttu-id="29432-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="29432-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29432-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="29432-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29432-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="29432-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29432-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="29432-126">Schema Name</span></span>  <br/> |<span data-ttu-id="29432-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="29432-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="29432-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="29432-128">Validation File</span></span>  <br/> |<span data-ttu-id="29432-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="29432-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29432-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="29432-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="29432-131">False</span><span class="sxs-lookup"><span data-stu-id="29432-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29432-132">См. также</span><span class="sxs-lookup"><span data-stu-id="29432-132">See also</span></span>



[<span data-ttu-id="29432-133">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="29432-133">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="29432-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="29432-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

