---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: Элемент CreateManagedFolder определяет запрос на добавление настраиваемых управляемых папок почтового ящика.
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761908"
---
# <a name="createmanagedfolder"></a><span data-ttu-id="f3b9e-103">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="f3b9e-103">CreateManagedFolder</span></span>

<span data-ttu-id="f3b9e-104">Элемент **CreateManagedFolder** определяет запрос на добавление настраиваемых управляемых папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-104">The **CreateManagedFolder** element defines a request to add managed custom folders to a mailbox.</span></span> 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 <span data-ttu-id="f3b9e-105">**CreateManagedFolderRequestType**</span><span class="sxs-lookup"><span data-stu-id="f3b9e-105">**CreateManagedFolderRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3b9e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3b9e-106">Attributes and elements</span></span>

<span data-ttu-id="f3b9e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3b9e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3b9e-108">Attributes</span></span>

<span data-ttu-id="f3b9e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3b9e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3b9e-110">Child elements</span></span>

|<span data-ttu-id="f3b9e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f3b9e-111">**Element**</span></span>|<span data-ttu-id="f3b9e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3b9e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3b9e-113">FolderNames</span><span class="sxs-lookup"><span data-stu-id="f3b9e-113">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="f3b9e-114">Содержит массив именованных управляемые папки для добавления к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-114">Contains an array of named managed folders to add to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f3b9e-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="f3b9e-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="f3b9e-116">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3b9e-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3b9e-117">Parent elements</span></span>

<span data-ttu-id="f3b9e-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3b9e-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="f3b9e-119">Remarks</span></span>

<span data-ttu-id="f3b9e-120">Учетная запись пользователя, отправившего запрос необходимы разрешения FullAccess для почтового ящика, где создаются управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-120">The account of the person who is making the request must have FullAccess permissions on the mailbox where the managed folders are created.</span></span> <span data-ttu-id="f3b9e-121">Параметр _ _ - AccessRights можно использовать с помощью командной консоли Exchange **Add-MailboxPermission** используется для назначения разрешений FullAccess.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-121">You can use the _ -AccessRights _ parameter with the Exchange Management Shell **Add-MailboxPermission** cmdlet to assign the FullAccess permission.</span></span> 
  
<span data-ttu-id="f3b9e-122">Несмотря на то, что веб-служб Exchange можно использовать для добавления управляемых папок для почтового ящика, нельзя использовать веб-служб Exchange для доступа к списку управляемых папок, которые доступны.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-122">Although you can use Exchange Web Services to add managed folders to a mailbox, you cannot use Exchange Web Services to access the list of managed folders that are available.</span></span> <span data-ttu-id="f3b9e-123">Для получения списка доступных управляемых папок, используйте командлет **get-managedfolder** Командная консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-123">To obtain a list of available managed folders, use the **get-managedfolder** Exchange Management Shell cmdlet.</span></span> <span data-ttu-id="f3b9e-124">Список, который возвращается с помощью **командлета get-managedfolder** будет содержать управляемые настраиваемые папки и управляемые папки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-124">The list that is returned by the **get-managedfolder cmdlet** will contain both managed custom folders and managed default folders.</span></span> <span data-ttu-id="f3b9e-125">Только могут добавлять папки из типа **managedcustomfolder** к почтовому ящику с помощью операции CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-125">You can only add folders of type **managedcustomfolder** to the mailbox by using the CreateManagedFolder operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f3b9e-126">Список управляемых папок можно также получить с помощью API DirectoryServices платформы Microsoft .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-126">You can also get a list of managed folders by using the DirectoryServices API of the Microsoft .NET Framework.</span></span> 
  
<span data-ttu-id="f3b9e-127">[Операция FindFolder](findfolder-operation.md) можно использовать для поиска управляемых папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-127">You can use the [FindFolder operation](findfolder-operation.md) to find managed folders in a mailbox.</span></span> <span data-ttu-id="f3b9e-128">Управляемые папки можно отличить путем установки для параметра элемент [BaseShape](baseshape.md) AllProperties в запросе.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-128">Managed folders can be distinguished by setting the [BaseShape](baseshape.md) element to AllProperties in the request.</span></span> <span data-ttu-id="f3b9e-129">Ответ будет содержать элемент [ManagedFolderInformation](managedfolderinformation.md) , чтобы отличать управляемых папок из папки хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-129">The response will contain a [ManagedFolderInformation](managedfolderinformation.md) element to distinguish the managed folders from the Exchange store folders.</span></span> <span data-ttu-id="f3b9e-130">Управляемые папки можно удалить точно так же, удалить другие типы папки.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-130">You can delete managed folders in the same manner that you delete other folder types.</span></span> 
  
<span data-ttu-id="f3b9e-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f3b9e-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3b9e-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3b9e-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3b9e-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3b9e-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3b9e-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3b9e-134">Schema Name</span></span>  <br/> |<span data-ttu-id="f3b9e-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f3b9e-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3b9e-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3b9e-136">Validation File</span></span>  <br/> |<span data-ttu-id="f3b9e-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f3b9e-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3b9e-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3b9e-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3b9e-139">False</span><span class="sxs-lookup"><span data-stu-id="f3b9e-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3b9e-140">См. также</span><span class="sxs-lookup"><span data-stu-id="f3b9e-140">See also</span></span>



[<span data-ttu-id="f3b9e-141">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="f3b9e-141">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
[<span data-ttu-id="f3b9e-142">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="f3b9e-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="f3b9e-143">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="f3b9e-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="f3b9e-144">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="f3b9e-144">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

