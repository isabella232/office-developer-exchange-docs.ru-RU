---
title: канделете
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
description: Элемент Канделете указывает, может ли клиент удалить управляемую папку.
ms.openlocfilehash: 5fe16c276bdb0c5b3b73ca63099559d3e869db3e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461592"
---
# <a name="candelete"></a><span data-ttu-id="b081e-103">канделете</span><span class="sxs-lookup"><span data-stu-id="b081e-103">CanDelete</span></span>

<span data-ttu-id="b081e-104">Элемент **канделете** указывает, может ли клиент удалить управляемую папку.</span><span class="sxs-lookup"><span data-stu-id="b081e-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="b081e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b081e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b081e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b081e-106">Attributes and elements</span></span>

<span data-ttu-id="b081e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b081e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b081e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b081e-108">Attributes</span></span>

<span data-ttu-id="b081e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b081e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b081e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b081e-110">Child elements</span></span>

<span data-ttu-id="b081e-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b081e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b081e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b081e-112">Parent elements</span></span>

|<span data-ttu-id="b081e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b081e-113">**Element**</span></span>|<span data-ttu-id="b081e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b081e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b081e-115">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="b081e-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="b081e-116">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="b081e-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b081e-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b081e-117">Text value</span></span>

<span data-ttu-id="b081e-118">При наличии этого элемента необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="b081e-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="b081e-119">Значение **true** указывает, что папку можно удалить; значение **false** означает, что папка не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="b081e-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b081e-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="b081e-120">Remarks</span></span>

<span data-ttu-id="b081e-121">Чтобы удалить управляемую папку, используйте [операцию DeleteFolder](deletefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b081e-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="b081e-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b081e-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b081e-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b081e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b081e-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b081e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b081e-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b081e-125">Schema name</span></span>  <br/> |<span data-ttu-id="b081e-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b081e-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="b081e-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b081e-127">Validation file</span></span>  <br/> |<span data-ttu-id="b081e-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b081e-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b081e-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b081e-129">Can be empty</span></span>  <br/> |<span data-ttu-id="b081e-130">False</span><span class="sxs-lookup"><span data-stu-id="b081e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b081e-131">См. также</span><span class="sxs-lookup"><span data-stu-id="b081e-131">See also</span></span>



[<span data-ttu-id="b081e-132">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="b081e-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="b081e-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b081e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b081e-134">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="b081e-134">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

