---
title: фолдернамес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderNames
api_type:
- schema
ms.assetid: 6cbe4083-5705-4695-a54e-8dab3e472662
description: Элемент Фолдернамес содержит массив именованных управляемых папок для добавления к почтовому ящику.
ms.openlocfilehash: 00cb1a81f420469033ccbc745313d2719b155aff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530988"
---
# <a name="foldernames"></a><span data-ttu-id="6491e-103">фолдернамес</span><span class="sxs-lookup"><span data-stu-id="6491e-103">FolderNames</span></span>

<span data-ttu-id="6491e-104">Элемент **фолдернамес** содержит массив именованных управляемых папок для добавления к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="6491e-104">The **FolderNames** element contains an array of named managed folders to add to a mailbox.</span></span> 
  
[<span data-ttu-id="6491e-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="6491e-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="6491e-106">фолдернамес</span><span class="sxs-lookup"><span data-stu-id="6491e-106">FolderNames</span></span>](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 <span data-ttu-id="6491e-107">**нонемптяррайоффолдернаместипе**</span><span class="sxs-lookup"><span data-stu-id="6491e-107">**NonEmptyArrayOfFolderNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6491e-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6491e-108">Attributes and elements</span></span>

<span data-ttu-id="6491e-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6491e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6491e-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6491e-110">Attributes</span></span>

<span data-ttu-id="6491e-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6491e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6491e-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6491e-112">Child elements</span></span>

|<span data-ttu-id="6491e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6491e-113">**Element**</span></span>|<span data-ttu-id="6491e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6491e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6491e-115">FolderName</span><span class="sxs-lookup"><span data-stu-id="6491e-115">FolderName</span></span>](foldername.md) <br/> |<span data-ttu-id="6491e-116">Определяет единую управляемую папку для добавления к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="6491e-116">Identifies a single managed folder to add to mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6491e-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6491e-117">Parent elements</span></span>

|<span data-ttu-id="6491e-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6491e-118">**Element**</span></span>|<span data-ttu-id="6491e-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6491e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6491e-120">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="6491e-120">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="6491e-121">Корневой элемент запроса на добавление управляемой папки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="6491e-121">The root element in a request to add a managed folder to a mailbox.</span></span>  <br/> <span data-ttu-id="6491e-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="6491e-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6491e-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="6491e-123">Remarks</span></span>

<span data-ttu-id="6491e-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6491e-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6491e-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6491e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6491e-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6491e-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6491e-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6491e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6491e-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6491e-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6491e-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6491e-129">Validation File</span></span>  <br/> |<span data-ttu-id="6491e-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6491e-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6491e-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6491e-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6491e-132">False</span><span class="sxs-lookup"><span data-stu-id="6491e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6491e-133">См. также</span><span class="sxs-lookup"><span data-stu-id="6491e-133">See also</span></span>



[<span data-ttu-id="6491e-134">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="6491e-134">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="6491e-135">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="6491e-135">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="6491e-136">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="6491e-136">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

