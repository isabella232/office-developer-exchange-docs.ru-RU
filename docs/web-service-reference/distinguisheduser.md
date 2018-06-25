---
title: DistinguishedUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedUser
api_type:
- schema
ms.assetid: 9362699d-666a-4acf-8fa1-c6669f0a2ae5
description: Элемент DistinguishedUser определяет учетные записи пользователей анонимные пользователи и по умолчанию для доступа делегата. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: b14be22bfe5316b9ab254e63cdfa0757596b8b92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762189"
---
# <a name="distinguisheduser"></a><span data-ttu-id="860b9-104">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="860b9-104">DistinguishedUser</span></span>

<span data-ttu-id="860b9-105">Элемент **DistinguishedUser** определяет учетные записи пользователей анонимные пользователи и по умолчанию для доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="860b9-105">The **DistinguishedUser** element identifies Anonymous and Default user accounts for delegate access.</span></span> <span data-ttu-id="860b9-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="860b9-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 <span data-ttu-id="860b9-107">**DistinguishedUserType**</span><span class="sxs-lookup"><span data-stu-id="860b9-107">**DistinguishedUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="860b9-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="860b9-108">Attributes and elements</span></span>

<span data-ttu-id="860b9-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="860b9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="860b9-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="860b9-110">Attributes</span></span>

<span data-ttu-id="860b9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="860b9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="860b9-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="860b9-112">Child elements</span></span>

<span data-ttu-id="860b9-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="860b9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="860b9-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="860b9-114">Parent elements</span></span>

|<span data-ttu-id="860b9-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="860b9-115">**Element**</span></span>|<span data-ttu-id="860b9-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="860b9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="860b9-117">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="860b9-117">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="860b9-118">Идентифицирует пользователя делегатом или пользователь, имеющий права доступа к папкам.</span><span class="sxs-lookup"><span data-stu-id="860b9-118">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="860b9-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="860b9-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="860b9-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="860b9-120">Text value</span></span>

<span data-ttu-id="860b9-121">Текстовое значение **по умолчанию** описание по умолчанию для пользователей делегата, добавленный к почтовому ящику участника.</span><span class="sxs-lookup"><span data-stu-id="860b9-121">A text value of **Default** describes the default setting for delegate users who are added to the principal's mailbox.</span></span> <span data-ttu-id="860b9-122">Текстовое значение **Anonymous** описываются параметры доступа делегата, анонимных пользователей от основного сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="860b9-122">A text value of **Anonymous** describes the delegate access settings that anonymous users have on the principal's mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="860b9-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="860b9-123">Remarks</span></span>

<span data-ttu-id="860b9-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="860b9-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="860b9-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="860b9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="860b9-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="860b9-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="860b9-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="860b9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="860b9-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="860b9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="860b9-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="860b9-129">Validation File</span></span>  <br/> |<span data-ttu-id="860b9-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="860b9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="860b9-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="860b9-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="860b9-132">False</span><span class="sxs-lookup"><span data-stu-id="860b9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="860b9-133">См. также</span><span class="sxs-lookup"><span data-stu-id="860b9-133">See also</span></span>

- [<span data-ttu-id="860b9-134">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="860b9-134">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="860b9-135">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="860b9-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="860b9-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="860b9-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="860b9-137">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="860b9-137">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

