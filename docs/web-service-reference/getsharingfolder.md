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
description: Элемент GetSharingFolder определяет запрос на получение идентификатора локальной папки указанной общей папки. Это базовый элемент для операции GetSharingFolder.
ms.openlocfilehash: cb76c534d9b30d0a9d1b267396551eb2871e638a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460507"
---
# <a name="getsharingfolder"></a><span data-ttu-id="9c8d7-104">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="9c8d7-104">GetSharingFolder</span></span>

<span data-ttu-id="9c8d7-105">Элемент **GetSharingFolder** определяет запрос на получение идентификатора локальной папки указанной общей папки.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-105">The **GetSharingFolder** element defines a request to get the local folder identifier of a specified shared folder.</span></span> <span data-ttu-id="9c8d7-106">Это базовый элемент для [операции GetSharingFolder](getsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9c8d7-106">It is the base element for the [GetSharingFolder operation](getsharingfolder-operation.md).</span></span>
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 <span data-ttu-id="9c8d7-107">**жетшарингфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="9c8d7-107">**GetSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c8d7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9c8d7-108">Attributes and elements</span></span>

<span data-ttu-id="9c8d7-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c8d7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9c8d7-110">Attributes</span></span>

<span data-ttu-id="9c8d7-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c8d7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9c8d7-112">Child elements</span></span>

|<span data-ttu-id="9c8d7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c8d7-113">**Element**</span></span>|<span data-ttu-id="9c8d7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c8d7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c8d7-115">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="9c8d7-115">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="9c8d7-116">Представляет SMTP-адрес электронной почты другой стороны в отношении совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-116">Represents the SMTP e-mail address of the other party in the sharing relationship.</span></span> <span data-ttu-id="9c8d7-117">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="9c8d7-118">DataType</span><span class="sxs-lookup"><span data-stu-id="9c8d7-118">DataType</span></span>](datatype.md) <br/> |<span data-ttu-id="9c8d7-119">Описывает тип данных, к которым предоставлен общий доступ в общей папке.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-119">Describes the type of data that is shared by a shared folder.</span></span> <span data-ttu-id="9c8d7-120">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9c8d7-121">шаредфолдерид</span><span class="sxs-lookup"><span data-stu-id="9c8d7-121">SharedFolderId</span></span>](sharedfolderid.md) <br/> |<span data-ttu-id="9c8d7-122">Представляет идентификатор общей папки, для которой должен быть возвращен идентификатор локальной папки.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-122">Represents the identifier of the shared folder whose local folder identifier should be returned.</span></span> <span data-ttu-id="9c8d7-123">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-123">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c8d7-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9c8d7-124">Parent elements</span></span>

<span data-ttu-id="9c8d7-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c8d7-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="9c8d7-126">Remarks</span></span>

<span data-ttu-id="9c8d7-127">Элемент GetSharingFolder должен содержать элемент [SmtpAddress](smtpaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="9c8d7-127">A GetSharingFolder element must contain an [SmtpAddress](smtpaddress.md) element.</span></span> <span data-ttu-id="9c8d7-128">Элемент GetSharingFolder также должен содержать либо элемент [DataType](datatype.md) , либо элемент [шаредфолдерид](sharedfolderid.md) , но не может содержать и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-128">A GetSharingFolder element must also contain either a [DataType](datatype.md) element or a [SharedFolderId](sharedfolderid.md) element, but cannot contain both.</span></span> 
  
<span data-ttu-id="9c8d7-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9c8d7-129">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c8d7-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9c8d7-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c8d7-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9c8d7-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9c8d7-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9c8d7-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9c8d7-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9c8d7-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9c8d7-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9c8d7-134">Validation File</span></span>  <br/> |<span data-ttu-id="9c8d7-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9c8d7-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c8d7-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9c8d7-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c8d7-137">False</span><span class="sxs-lookup"><span data-stu-id="9c8d7-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c8d7-138">См. также</span><span class="sxs-lookup"><span data-stu-id="9c8d7-138">See also</span></span>



[<span data-ttu-id="9c8d7-139">Операция GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="9c8d7-139">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="9c8d7-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9c8d7-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

