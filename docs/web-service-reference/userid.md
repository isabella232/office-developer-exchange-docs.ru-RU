---
title: UserId
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
description: Элемент UserId идентифицирует пользователя делегата или пользователя с разрешениями на доступ к папке.
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840421"
---
# <a name="userid"></a><span data-ttu-id="1fea3-103">UserId</span><span class="sxs-lookup"><span data-stu-id="1fea3-103">UserId</span></span>

<span data-ttu-id="1fea3-104">Элемент **UserID** идентифицирует пользователя делегата или пользователя с разрешениями на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="1fea3-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="1fea3-105">**усеридтипе**</span><span class="sxs-lookup"><span data-stu-id="1fea3-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fea3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1fea3-106">Attributes and elements</span></span>

<span data-ttu-id="1fea3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1fea3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fea3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1fea3-108">Attributes</span></span>

<span data-ttu-id="1fea3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1fea3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fea3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1fea3-110">Child elements</span></span>

|<span data-ttu-id="1fea3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1fea3-111">**Element**</span></span>|<span data-ttu-id="1fea3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1fea3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fea3-113">SID</span><span class="sxs-lookup"><span data-stu-id="1fea3-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="1fea3-114">Представляет форму языка определения дескрипторов безопасности (SID).</span><span class="sxs-lookup"><span data-stu-id="1fea3-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="1fea3-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1fea3-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="1fea3-116">Представляет основной SMTP-адрес учетной записи, которая будет использоваться для делегирования доступа.</span><span class="sxs-lookup"><span data-stu-id="1fea3-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="1fea3-117">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="1fea3-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="1fea3-118">Определяет отображаемое имя папки, контакта, списка рассылки или пользователя делегата.</span><span class="sxs-lookup"><span data-stu-id="1fea3-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="1fea3-119">дистингуишедусер</span><span class="sxs-lookup"><span data-stu-id="1fea3-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="1fea3-120">Определяет анонимные и учетные записи пользователей по умолчанию для делегирования доступа.</span><span class="sxs-lookup"><span data-stu-id="1fea3-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="1fea3-121">екстерналусеридентити</span><span class="sxs-lookup"><span data-stu-id="1fea3-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="1fea3-122">Определяет внешнего пользователя делегата или внешнего пользователя с разрешениями на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="1fea3-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1fea3-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1fea3-123">Parent elements</span></span>

|<span data-ttu-id="1fea3-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1fea3-124">**Element**</span></span>|<span data-ttu-id="1fea3-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1fea3-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fea3-126">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="1fea3-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="1fea3-127">Определяет одного делегата для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1fea3-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1fea3-128">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1fea3-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="1fea3-129">Определяет доступ пользователя к папке.</span><span class="sxs-lookup"><span data-stu-id="1fea3-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="1fea3-130">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="1fea3-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="1fea3-131">Определяет доступ пользователя к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="1fea3-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="1fea3-132">UserIds</span><span class="sxs-lookup"><span data-stu-id="1fea3-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="1fea3-133">Содержит массив делегированных пользователей, которые необходимо получить или удалить из почтового ящика участника.</span><span class="sxs-lookup"><span data-stu-id="1fea3-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1fea3-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1fea3-134">Text value</span></span>

<span data-ttu-id="1fea3-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="1fea3-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1fea3-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="1fea3-136">Remarks</span></span>

<span data-ttu-id="1fea3-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1fea3-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fea3-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1fea3-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fea3-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1fea3-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1fea3-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1fea3-140">Schema Name</span></span>  <br/> |<span data-ttu-id="1fea3-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1fea3-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="1fea3-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1fea3-142">Validation File</span></span>  <br/> |<span data-ttu-id="1fea3-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1fea3-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1fea3-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1fea3-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="1fea3-145">False</span><span class="sxs-lookup"><span data-stu-id="1fea3-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1fea3-146">См. также</span><span class="sxs-lookup"><span data-stu-id="1fea3-146">See also</span></span>



[<span data-ttu-id="1fea3-147">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="1fea3-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="1fea3-148">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="1fea3-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="1fea3-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1fea3-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1fea3-150">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="1fea3-150">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

