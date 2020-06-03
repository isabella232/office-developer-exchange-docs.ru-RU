---
title: шарингфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: Элемент Шарингфолдерид представляет идентификатор локальной папки в отношении общего доступа.
ms.openlocfilehash: 02780251639ee651ca65d8eadded43260852aaf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526580"
---
# <a name="sharingfolderid"></a><span data-ttu-id="bc922-103">шарингфолдерид</span><span class="sxs-lookup"><span data-stu-id="bc922-103">SharingFolderId</span></span>

<span data-ttu-id="bc922-104">Элемент **шарингфолдерид** представляет идентификатор локальной папки в отношении общего доступа.</span><span class="sxs-lookup"><span data-stu-id="bc922-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="bc922-105">**фолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="bc922-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc922-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc922-106">Attributes and elements</span></span>

<span data-ttu-id="bc922-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc922-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc922-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc922-108">Attributes</span></span>

|<span data-ttu-id="bc922-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bc922-109">**Attribute**</span></span>|<span data-ttu-id="bc922-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc922-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc922-111">Id</span><span class="sxs-lookup"><span data-stu-id="bc922-111">Id</span></span>  <br/> |<span data-ttu-id="bc922-112">Содержит строку, определяющую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc922-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="bc922-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bc922-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="bc922-114">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="bc922-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="bc922-115">Содержит строку, определяющую версию папки, определяемую атрибутом ID.</span><span class="sxs-lookup"><span data-stu-id="bc922-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="bc922-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bc922-116">This attribute is optional.</span></span> <span data-ttu-id="bc922-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.</span><span class="sxs-lookup"><span data-stu-id="bc922-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bc922-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc922-118">Child elements</span></span>

<span data-ttu-id="bc922-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc922-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc922-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc922-120">Parent elements</span></span>

|<span data-ttu-id="bc922-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc922-121">**Element**</span></span>|<span data-ttu-id="bc922-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc922-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc922-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="bc922-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="bc922-124">Определяет запрос на обновление указанной локальной папки.</span><span class="sxs-lookup"><span data-stu-id="bc922-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="bc922-125">жетшарингфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="bc922-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="bc922-126">Определяет ответ на запрос [операции GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc922-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="bc922-127">жетшарингфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bc922-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="bc922-128">Содержит состояние и результат одного запроса [операции GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc922-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc922-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc922-129">Remarks</span></span>

<span data-ttu-id="bc922-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bc922-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc922-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc922-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc922-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc922-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc922-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc922-133">Schema Name</span></span>  <br/> |<span data-ttu-id="bc922-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bc922-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc922-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc922-135">Validation File</span></span>  <br/> |<span data-ttu-id="bc922-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc922-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc922-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc922-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc922-138">False</span><span class="sxs-lookup"><span data-stu-id="bc922-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc922-139">См. также</span><span class="sxs-lookup"><span data-stu-id="bc922-139">See also</span></span>



- [<span data-ttu-id="bc922-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc922-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

