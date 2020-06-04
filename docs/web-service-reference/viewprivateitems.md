---
title: виевприватеитемс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ViewPrivateItems
api_type:
- schema
ms.assetid: 80b949ac-440c-4a01-b428-ebafb5b1b802
description: Элемент Виевприватеитемс указывает, имеет ли представитель пользователя или клиентское приложение разрешение на просмотр частных элементов в почтовом ящике участника.
ms.openlocfilehash: 4e1375f7c4a3c660cc5de885deff8d094250ca7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44525971"
---
# <a name="viewprivateitems"></a><span data-ttu-id="1b423-103">виевприватеитемс</span><span class="sxs-lookup"><span data-stu-id="1b423-103">ViewPrivateItems</span></span>

<span data-ttu-id="1b423-104">Элемент **виевприватеитемс** указывает, имеет ли представитель пользователя или клиентское приложение разрешение на просмотр частных элементов в почтовом ящике участника.</span><span class="sxs-lookup"><span data-stu-id="1b423-104">The **ViewPrivateItems** element indicates whether a delegate user or client application has permission to view private items in the principal's mailbox.</span></span> 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 <span data-ttu-id="1b423-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1b423-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b423-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1b423-106">Attributes and elements</span></span>

<span data-ttu-id="1b423-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1b423-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b423-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1b423-108">Attributes</span></span>

<span data-ttu-id="1b423-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1b423-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b423-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1b423-110">Child elements</span></span>

<span data-ttu-id="1b423-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1b423-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b423-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1b423-112">Parent elements</span></span>

|<span data-ttu-id="1b423-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b423-113">**Element**</span></span>|<span data-ttu-id="1b423-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b423-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b423-115">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="1b423-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="1b423-116">Определяет одного делегата для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1b423-116">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1b423-117">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="1b423-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="1b423-118">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="1b423-118">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="1b423-119">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b423-119">This element is read-only.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b423-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1b423-120">Text value</span></span>

<span data-ttu-id="1b423-121">Значение **true** указывает, что делегат или клиент могут просматривать частные элементы в почтовом ящике участника.</span><span class="sxs-lookup"><span data-stu-id="1b423-121">A value of **true** indicates that the delegate or client can view private items in the principal's mailbox.</span></span> <span data-ttu-id="1b423-122">Значение **false** указывает, что закрытые элементы невидимы для делегата или клиента.</span><span class="sxs-lookup"><span data-stu-id="1b423-122">A value of **false** indicates that private items are not visible to a delegate or client.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1b423-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="1b423-123">Remarks</span></span>

<span data-ttu-id="1b423-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b423-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b423-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1b423-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b423-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1b423-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1b423-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1b423-127">Schema Name</span></span>  <br/> |<span data-ttu-id="1b423-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1b423-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="1b423-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1b423-129">Validation File</span></span>  <br/> |<span data-ttu-id="1b423-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1b423-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1b423-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1b423-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b423-132">False</span><span class="sxs-lookup"><span data-stu-id="1b423-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b423-133">См. также</span><span class="sxs-lookup"><span data-stu-id="1b423-133">See also</span></span>



[<span data-ttu-id="1b423-134">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="1b423-134">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="1b423-135">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="1b423-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="1b423-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b423-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1b423-137">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="1b423-137">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

