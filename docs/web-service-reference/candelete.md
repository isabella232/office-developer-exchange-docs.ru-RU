---
title: CanDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanDelete
api_type:
- schema
ms.assetid: 55e17121-aad0-4f90-889f-2c3512e9579c
description: Элемент CanDelete указывает, можно ли удалить управляемой папки клиентом.
ms.openlocfilehash: b70b28bd6b3c9452f5d7f249f453218d555754da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761665"
---
# <a name="candelete"></a><span data-ttu-id="7827f-103">CanDelete</span><span class="sxs-lookup"><span data-stu-id="7827f-103">CanDelete</span></span>

<span data-ttu-id="7827f-104">Элемент **CanDelete** указывает, можно ли удалить управляемой папки клиентом.</span><span class="sxs-lookup"><span data-stu-id="7827f-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="7827f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7827f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7827f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7827f-106">Attributes and elements</span></span>

<span data-ttu-id="7827f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7827f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7827f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7827f-108">Attributes</span></span>

<span data-ttu-id="7827f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7827f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7827f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7827f-110">Child elements</span></span>

<span data-ttu-id="7827f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7827f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7827f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7827f-112">Parent elements</span></span>

|<span data-ttu-id="7827f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7827f-113">**Element**</span></span>|<span data-ttu-id="7827f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7827f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7827f-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="7827f-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="7827f-116">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="7827f-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7827f-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7827f-117">Text value</span></span>

<span data-ttu-id="7827f-118">Текстовое значение, представляющее логическое значение является обязательным, если присутствует этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7827f-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="7827f-119">Значение **true** указывает, что можно удалить папку; значение **false** означает, что папка не может быть удален.</span><span class="sxs-lookup"><span data-stu-id="7827f-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7827f-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="7827f-120">Remarks</span></span>

<span data-ttu-id="7827f-121">Чтобы удалить управляемых папок, с помощью [операции DeleteFolder](deletefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7827f-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="7827f-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7827f-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7827f-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7827f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7827f-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7827f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7827f-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7827f-125">Schema name</span></span>  <br/> |<span data-ttu-id="7827f-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7827f-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="7827f-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7827f-127">Validation file</span></span>  <br/> |<span data-ttu-id="7827f-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7827f-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7827f-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7827f-129">Can be empty</span></span>  <br/> |<span data-ttu-id="7827f-130">False</span><span class="sxs-lookup"><span data-stu-id="7827f-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7827f-131">См. также</span><span class="sxs-lookup"><span data-stu-id="7827f-131">See also</span></span>



[<span data-ttu-id="7827f-132">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="7827f-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="7827f-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7827f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7827f-134">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="7827f-134">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

