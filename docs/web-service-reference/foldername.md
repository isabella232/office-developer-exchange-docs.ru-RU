---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: Элемент имя_папки определяет отдельную управляемую настраиваемую папку, добавляемую к почтовому ящику.
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762629"
---
# <a name="foldername"></a><span data-ttu-id="4b2f0-103">FolderName</span><span class="sxs-lookup"><span data-stu-id="4b2f0-103">FolderName</span></span>

<span data-ttu-id="4b2f0-104">Элемент **имя_папки** определяет отдельную управляемую настраиваемую папку, добавляемую к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-104">The **FolderName** element identifies a single managed custom folder to add to a mailbox.</span></span> 
  
[<span data-ttu-id="4b2f0-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="4b2f0-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="4b2f0-106">фолдернамес</span><span class="sxs-lookup"><span data-stu-id="4b2f0-106">FolderNames</span></span>](foldernames.md)
  
[<span data-ttu-id="4b2f0-107">FolderName</span><span class="sxs-lookup"><span data-stu-id="4b2f0-107">FolderName</span></span>](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 <span data-ttu-id="4b2f0-108">**строка**</span><span class="sxs-lookup"><span data-stu-id="4b2f0-108">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b2f0-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4b2f0-109">Attributes and elements</span></span>

<span data-ttu-id="4b2f0-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b2f0-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4b2f0-111">Attributes</span></span>

<span data-ttu-id="4b2f0-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b2f0-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4b2f0-113">Child elements</span></span>

<span data-ttu-id="4b2f0-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b2f0-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4b2f0-115">Parent elements</span></span>

|<span data-ttu-id="4b2f0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4b2f0-116">**Element**</span></span>|<span data-ttu-id="4b2f0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4b2f0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b2f0-118">фолдернамес</span><span class="sxs-lookup"><span data-stu-id="4b2f0-118">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="4b2f0-119">Содержит массив именованных управляемых настраиваемых папок для добавления к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-119">Contains an array of named managed custom folders to add to a mailbox.</span></span>  <br/> <span data-ttu-id="4b2f0-120">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="4b2f0-120">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4b2f0-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4b2f0-121">Text value</span></span>

<span data-ttu-id="4b2f0-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-122">A text value is required.</span></span> <span data-ttu-id="4b2f0-123">Текстовое значение представляет имя папки.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-123">The text value represents a folder name.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4b2f0-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="4b2f0-124">Remarks</span></span>

<span data-ttu-id="4b2f0-125">Несмотря на то, что вы можете использовать веб-службы Exchange для добавления управляемых настраиваемых папок в почтовый ящик, вы не можете использовать одну и ту же технологию для доступа к списку доступных управляемых настраиваемых папок.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-125">Although you can use Exchange Web Services to add managed custom folders to a mailbox, you cannot use the same technology to access the list of available managed custom folders.</span></span> <span data-ttu-id="4b2f0-126">Список управляемых настраиваемых папок можно получить с помощью команды командной консоли Exchange или API, с помощью которого выполняется взаимодействие с службой каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-126">You can obtain a list of managed custom folders by using an Exchange Management Shell command or by using an API that interfaces with the Active Directory directory service.</span></span> <span data-ttu-id="4b2f0-127">Имя папки — это имя соответствующего объекта Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-127">The folder name is the name of the corresponding Active Directory object.</span></span>
  
<span data-ttu-id="4b2f0-128">Для поиска управляемых настраиваемых папок можно использовать [операцию FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4b2f0-128">You can use the [FindFolder operation](findfolder-operation.md) to find managed custom folders.</span></span> <span data-ttu-id="4b2f0-129">Используйте [операцию DeleteFolder](deletefolder-operation.md) для удаления управляемых пользовательских папок.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-129">Use the [DeleteFolder operation](deletefolder-operation.md) to delete managed custom folders.</span></span> 
  
<span data-ttu-id="4b2f0-130">Важно отметить, что параметр **имя_папки** — это имя существующей управляемой настраиваемой папки в Организации.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-130">It is important to note that **FolderName** is the name of an existing managed custom folder in the organization.</span></span> <span data-ttu-id="4b2f0-131">При попытке добавить папку, которой нет в Организации, будет получено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-131">An attempt to add a folder that is not in the organization will result in an error response.</span></span> 
  
<span data-ttu-id="4b2f0-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4b2f0-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b2f0-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4b2f0-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b2f0-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4b2f0-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b2f0-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4b2f0-135">Schema Name</span></span>  <br/> |<span data-ttu-id="4b2f0-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4b2f0-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b2f0-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4b2f0-137">Validation File</span></span>  <br/> |<span data-ttu-id="4b2f0-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4b2f0-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b2f0-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4b2f0-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b2f0-140">False</span><span class="sxs-lookup"><span data-stu-id="4b2f0-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b2f0-141">См. также</span><span class="sxs-lookup"><span data-stu-id="4b2f0-141">See also</span></span>



[<span data-ttu-id="4b2f0-142">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="4b2f0-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="4b2f0-143">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="4b2f0-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="4b2f0-144">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="4b2f0-144">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

