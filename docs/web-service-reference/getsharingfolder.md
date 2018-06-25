---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: Элемент GetSharingFolder определяет запрос для получения идентификатора локальной папки указанной общей папке. Это базовый элемент для операции GetSharingFolder.
ms.openlocfilehash: 7c2f31aa27c1cbde6cdad2b41a341916b4bed2ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833669"
---
# <a name="getsharingfolder"></a><span data-ttu-id="88d24-104">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="88d24-104">GetSharingFolder</span></span>

<span data-ttu-id="88d24-105">Элемент **GetSharingFolder** определяет запрос для получения идентификатора локальной папки указанной общей папке.</span><span class="sxs-lookup"><span data-stu-id="88d24-105">The **GetSharingFolder** element defines a request to get the local folder identifier of a specified shared folder.</span></span> <span data-ttu-id="88d24-106">Это базовый элемент для [операции GetSharingFolder](getsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="88d24-106">It is the base element for the [GetSharingFolder operation](getsharingfolder-operation.md).</span></span>
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 <span data-ttu-id="88d24-107">**GetSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="88d24-107">**GetSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88d24-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88d24-108">Attributes and elements</span></span>

<span data-ttu-id="88d24-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="88d24-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88d24-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88d24-110">Attributes</span></span>

<span data-ttu-id="88d24-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="88d24-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88d24-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88d24-112">Child elements</span></span>

|<span data-ttu-id="88d24-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88d24-113">**Element**</span></span>|<span data-ttu-id="88d24-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88d24-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88d24-115">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="88d24-115">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="88d24-116">Представляет адрес электронной почты SMTP другой стороны в отношении общего доступа.</span><span class="sxs-lookup"><span data-stu-id="88d24-116">Represents the SMTP e-mail address of the other party in the sharing relationship.</span></span> <span data-ttu-id="88d24-117">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="88d24-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="88d24-118">Тип данных</span><span class="sxs-lookup"><span data-stu-id="88d24-118">DataType</span></span>](datatype.md) <br/> |<span data-ttu-id="88d24-119">Описывает тип данных, общий для общей папки.</span><span class="sxs-lookup"><span data-stu-id="88d24-119">Describes the type of data that is shared by a shared folder.</span></span> <span data-ttu-id="88d24-120">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="88d24-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="88d24-121">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="88d24-121">SharedFolderId</span></span>](sharedfolderid.md) <br/> |<span data-ttu-id="88d24-122">Представляет идентификатор общей папки, должны быть возвращены, идентификатор которого локальную папку.</span><span class="sxs-lookup"><span data-stu-id="88d24-122">Represents the identifier of the shared folder whose local folder identifier should be returned.</span></span> <span data-ttu-id="88d24-123">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="88d24-123">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88d24-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88d24-124">Parent elements</span></span>

<span data-ttu-id="88d24-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="88d24-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88d24-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="88d24-126">Remarks</span></span>

<span data-ttu-id="88d24-127">Элемент GetSharingFolder должен содержать элемент [SmtpAddress](smtpaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="88d24-127">A GetSharingFolder element must contain an [SmtpAddress](smtpaddress.md) element.</span></span> <span data-ttu-id="88d24-128">Элемент GetSharingFolder должен также содержать элемент [тип данных](datatype.md) или элемент [SharedFolderId](sharedfolderid.md) , но не может одновременно содержать.</span><span class="sxs-lookup"><span data-stu-id="88d24-128">A GetSharingFolder element must also contain either a [DataType](datatype.md) element or a [SharedFolderId](sharedfolderid.md) element, but cannot contain both.</span></span> 
  
<span data-ttu-id="88d24-129">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="88d24-129">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88d24-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88d24-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88d24-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88d24-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="88d24-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88d24-132">Schema Name</span></span>  <br/> |<span data-ttu-id="88d24-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="88d24-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="88d24-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88d24-134">Validation File</span></span>  <br/> |<span data-ttu-id="88d24-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88d24-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88d24-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88d24-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="88d24-137">False</span><span class="sxs-lookup"><span data-stu-id="88d24-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88d24-138">См. также</span><span class="sxs-lookup"><span data-stu-id="88d24-138">See also</span></span>



[<span data-ttu-id="88d24-139">Операция GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="88d24-139">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="88d24-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="88d24-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

