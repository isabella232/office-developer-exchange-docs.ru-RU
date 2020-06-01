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
description: Элемент RemoveDelegate определяет запрос на удаление делегатов из почтового ящика. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: eca357ad1ed2dc692f9f192b97abd3a5d765fafb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465522"
---
# <a name="removedelegate"></a><span data-ttu-id="c3ffb-104">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="c3ffb-104">RemoveDelegate</span></span>

<span data-ttu-id="c3ffb-105">Элемент **RemoveDelegate** определяет запрос на удаление делегатов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-105">The **RemoveDelegate** element defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="c3ffb-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c3ffb-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<RemoveDelegate>
      <Mailbox/>
   <UserIds/>
</RemoveDelegate>
```

 <span data-ttu-id="c3ffb-107">**ремоведелегатетипе**</span><span class="sxs-lookup"><span data-stu-id="c3ffb-107">**RemoveDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3ffb-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c3ffb-108">Attributes and elements</span></span>

<span data-ttu-id="c3ffb-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3ffb-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c3ffb-110">Attributes</span></span>

<span data-ttu-id="c3ffb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3ffb-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c3ffb-112">Child elements</span></span>

|<span data-ttu-id="c3ffb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c3ffb-113">**Element**</span></span>|<span data-ttu-id="c3ffb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c3ffb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3ffb-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="c3ffb-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c3ffb-116">Определяет почтовый ящик субъекта.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-116">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c3ffb-117">UserIds</span><span class="sxs-lookup"><span data-stu-id="c3ffb-117">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="c3ffb-118">Содержит массив делегированных пользователей, которые необходимо удалить из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-118">Contains an array of delegate users to remove from a principal's mailbox.</span></span> <span data-ttu-id="c3ffb-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c3ffb-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c3ffb-120">Parent elements</span></span>

<span data-ttu-id="c3ffb-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c3ffb-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="c3ffb-122">Remarks</span></span>

<span data-ttu-id="c3ffb-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c3ffb-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3ffb-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c3ffb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3ffb-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c3ffb-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c3ffb-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c3ffb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c3ffb-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c3ffb-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c3ffb-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c3ffb-128">Validation File</span></span>  <br/> |<span data-ttu-id="c3ffb-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c3ffb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c3ffb-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c3ffb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c3ffb-131">False</span><span class="sxs-lookup"><span data-stu-id="c3ffb-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c3ffb-132">См. также</span><span class="sxs-lookup"><span data-stu-id="c3ffb-132">See also</span></span>



[<span data-ttu-id="c3ffb-133">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="c3ffb-133">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="c3ffb-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c3ffb-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

