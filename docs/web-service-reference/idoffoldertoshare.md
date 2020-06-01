---
title: идоффолдертошаре
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
description: Элемент Идоффолдертошаре представляет идентификатор папки на сервере, к которой будет предоставлен общий доступ.
ms.openlocfilehash: 93a4740d9adefbb35aae071f0a6bfcb4b2021b4d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457629"
---
# <a name="idoffoldertoshare"></a><span data-ttu-id="26666-103">идоффолдертошаре</span><span class="sxs-lookup"><span data-stu-id="26666-103">IdOfFolderToShare</span></span>

<span data-ttu-id="26666-104">Элемент **идоффолдертошаре** представляет идентификатор папки на сервере, к которой будет предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="26666-104">The **IdOfFolderToShare** element represents the identifier of the folder on the server that will be shared.</span></span> 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 <span data-ttu-id="26666-105">**фолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="26666-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26666-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="26666-106">Attributes and elements</span></span>

<span data-ttu-id="26666-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="26666-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26666-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="26666-108">Attributes</span></span>

|<span data-ttu-id="26666-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="26666-109">**Attribute**</span></span>|<span data-ttu-id="26666-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26666-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="26666-111">Id</span><span class="sxs-lookup"><span data-stu-id="26666-111">Id</span></span>  <br/> |<span data-ttu-id="26666-112">Содержит строку, определяющую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="26666-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="26666-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="26666-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="26666-114">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="26666-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="26666-115">Содержит строку, определяющую версию папки, определяемую атрибутом ID.</span><span class="sxs-lookup"><span data-stu-id="26666-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="26666-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="26666-116">This attribute is optional.</span></span> <span data-ttu-id="26666-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.</span><span class="sxs-lookup"><span data-stu-id="26666-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="26666-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="26666-118">Child elements</span></span>

<span data-ttu-id="26666-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="26666-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26666-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="26666-120">Parent elements</span></span>

|<span data-ttu-id="26666-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="26666-121">**Element**</span></span>|<span data-ttu-id="26666-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26666-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26666-123">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="26666-123">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="26666-124">Определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="26666-124">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26666-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="26666-125">Remarks</span></span>

<span data-ttu-id="26666-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="26666-126">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26666-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="26666-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26666-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="26666-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26666-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="26666-129">Schema Name</span></span>  <br/> |<span data-ttu-id="26666-130">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="26666-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26666-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="26666-131">Validation File</span></span>  <br/> |<span data-ttu-id="26666-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="26666-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26666-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="26666-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="26666-134">False</span><span class="sxs-lookup"><span data-stu-id="26666-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26666-135">См. также</span><span class="sxs-lookup"><span data-stu-id="26666-135">See also</span></span>



[<span data-ttu-id="26666-136">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="26666-136">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="26666-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="26666-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

