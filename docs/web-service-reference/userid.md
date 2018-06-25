---
title: ИД пользователя
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: Элемент UserId определяет представитель или пользователь, имеющий права доступа к папкам.
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840421"
---
# <a name="userid"></a><span data-ttu-id="5a3d2-103">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="5a3d2-103">UserId</span></span>

<span data-ttu-id="5a3d2-104">Элемент **UserId** определяет представитель или пользователь, имеющий права доступа к папкам.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="5a3d2-105">**UserIdType**</span><span class="sxs-lookup"><span data-stu-id="5a3d2-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a3d2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5a3d2-106">Attributes and elements</span></span>

<span data-ttu-id="5a3d2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a3d2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5a3d2-108">Attributes</span></span>

<span data-ttu-id="5a3d2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a3d2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5a3d2-110">Child elements</span></span>

|<span data-ttu-id="5a3d2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5a3d2-111">**Element**</span></span>|<span data-ttu-id="5a3d2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5a3d2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a3d2-113">ИД БЕЗОПАСНОСТИ</span><span class="sxs-lookup"><span data-stu-id="5a3d2-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="5a3d2-114">Представляет идентификатор безопасности (SID) формы языке SDDL определения дескриптора безопасности.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="5a3d2-115">Параметр PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5a3d2-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="5a3d2-116">Представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, которое будет использоваться для доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="5a3d2-117">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="5a3d2-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="5a3d2-118">Задает отображаемое имя папки, контактов, список рассылки или делегата.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="5a3d2-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="5a3d2-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="5a3d2-120">Определяет учетные записи пользователей анонимные пользователи и по умолчанию для доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="5a3d2-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="5a3d2-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="5a3d2-122">Идентифицирует пользователя с внешним делегат или внешний пользователь, имеющий права доступа к папкам.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5a3d2-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5a3d2-123">Parent elements</span></span>

|<span data-ttu-id="5a3d2-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5a3d2-124">**Element**</span></span>|<span data-ttu-id="5a3d2-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5a3d2-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a3d2-126">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="5a3d2-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="5a3d2-127">Определяет один делегат для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5a3d2-128">Разрешение</span><span class="sxs-lookup"><span data-stu-id="5a3d2-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="5a3d2-129">Определяет доступ пользователя к папке.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="5a3d2-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="5a3d2-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="5a3d2-131">Определяет доступ пользователя к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="5a3d2-132">UserIds</span><span class="sxs-lookup"><span data-stu-id="5a3d2-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="5a3d2-133">Содержит массив делегат пользователям получить или удалить из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a3d2-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5a3d2-134">Text value</span></span>

<span data-ttu-id="5a3d2-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5a3d2-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="5a3d2-136">Remarks</span></span>

<span data-ttu-id="5a3d2-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a3d2-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a3d2-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5a3d2-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a3d2-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5a3d2-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a3d2-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5a3d2-140">Schema Name</span></span>  <br/> |<span data-ttu-id="5a3d2-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5a3d2-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a3d2-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5a3d2-142">Validation File</span></span>  <br/> |<span data-ttu-id="5a3d2-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a3d2-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a3d2-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5a3d2-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a3d2-145">False</span><span class="sxs-lookup"><span data-stu-id="5a3d2-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a3d2-146">См. также</span><span class="sxs-lookup"><span data-stu-id="5a3d2-146">See also</span></span>



[<span data-ttu-id="5a3d2-147">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="5a3d2-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="5a3d2-148">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="5a3d2-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="5a3d2-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5a3d2-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5a3d2-150">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="5a3d2-150">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

