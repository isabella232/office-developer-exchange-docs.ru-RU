---
title: IdOfFolderToShare
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IdOfFolderToShare
api_type:
- schema
ms.assetid: 199d1839-f061-4070-a977-874b0c08e5be
description: Элемент IdOfFolderToShare представляет идентификатор папки на сервере, который будет использоваться.
ms.openlocfilehash: 1e3e53819f23bbc5753ac21b9e3ea6593ac4826c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833853"
---
# <a name="idoffoldertoshare"></a><span data-ttu-id="9acf2-103">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="9acf2-103">IdOfFolderToShare</span></span>

<span data-ttu-id="9acf2-104">Элемент **IdOfFolderToShare** представляет идентификатор папки на сервере, который будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="9acf2-104">The **IdOfFolderToShare** element represents the identifier of the folder on the server that will be shared.</span></span> 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 <span data-ttu-id="9acf2-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="9acf2-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9acf2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9acf2-106">Attributes and elements</span></span>

<span data-ttu-id="9acf2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9acf2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9acf2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9acf2-108">Attributes</span></span>

|<span data-ttu-id="9acf2-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9acf2-109">**Attribute**</span></span>|<span data-ttu-id="9acf2-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9acf2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9acf2-111">Id</span><span class="sxs-lookup"><span data-stu-id="9acf2-111">Id</span></span>  <br/> |<span data-ttu-id="9acf2-112">Содержит строку, которая определяет папке в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9acf2-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="9acf2-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="9acf2-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="9acf2-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="9acf2-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="9acf2-115">Содержит строку, которая определяет к папке, которая определена в атрибуте Id версии.</span><span class="sxs-lookup"><span data-stu-id="9acf2-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="9acf2-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9acf2-116">This attribute is optional.</span></span> <span data-ttu-id="9acf2-117">Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.</span><span class="sxs-lookup"><span data-stu-id="9acf2-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9acf2-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9acf2-118">Child elements</span></span>

<span data-ttu-id="9acf2-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="9acf2-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9acf2-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9acf2-120">Parent elements</span></span>

|<span data-ttu-id="9acf2-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9acf2-121">**Element**</span></span>|<span data-ttu-id="9acf2-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9acf2-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9acf2-123">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="9acf2-123">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="9acf2-124">Определяет запрос на получение маркера непрозрачный проверки подлинности, идентифицирующее приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="9acf2-124">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9acf2-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="9acf2-125">Remarks</span></span>

<span data-ttu-id="9acf2-126">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9acf2-126">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9acf2-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9acf2-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9acf2-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9acf2-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9acf2-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9acf2-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9acf2-130">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9acf2-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9acf2-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9acf2-131">Validation File</span></span>  <br/> |<span data-ttu-id="9acf2-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9acf2-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9acf2-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9acf2-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9acf2-134">False</span><span class="sxs-lookup"><span data-stu-id="9acf2-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9acf2-135">См. также</span><span class="sxs-lookup"><span data-stu-id="9acf2-135">See also</span></span>



[<span data-ttu-id="9acf2-136">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="9acf2-136">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="9acf2-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9acf2-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

