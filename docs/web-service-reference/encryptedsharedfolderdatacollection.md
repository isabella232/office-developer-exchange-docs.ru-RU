---
title: EncryptedSharedFolderDataCollection
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderDataCollection
api_type:
- schema
ms.assetid: 25c6ae87-bbb9-4dd5-a85a-d669fcea137f
description: Элемент EncryptedSharedFolderDataCollection содержит коллекцию структур данных, которые клиент может использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.
ms.openlocfilehash: e4d37f5df10f5e270be5126479485239f2205d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762331"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="3dcea-103">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="3dcea-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="3dcea-104">Элемент **EncryptedSharedFolderDataCollection** содержит коллекцию структур данных, которые клиент может использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.</span><span class="sxs-lookup"><span data-stu-id="3dcea-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="3dcea-105">**ArrayOfEncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="3dcea-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3dcea-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3dcea-106">Attributes and elements</span></span>

<span data-ttu-id="3dcea-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3dcea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dcea-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3dcea-108">Attributes</span></span>

<span data-ttu-id="3dcea-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3dcea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dcea-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3dcea-110">Child elements</span></span>

|<span data-ttu-id="3dcea-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3dcea-111">**Element**</span></span>|<span data-ttu-id="3dcea-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3dcea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dcea-113">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="3dcea-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="3dcea-114">Содержит зашифрованные данные, которые клиент может использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.</span><span class="sxs-lookup"><span data-stu-id="3dcea-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3dcea-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3dcea-115">Parent elements</span></span>

|<span data-ttu-id="3dcea-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3dcea-116">**Element**</span></span>|<span data-ttu-id="3dcea-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3dcea-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dcea-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="3dcea-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="3dcea-119">Определяет ответ на запрос [Операция GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3dcea-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="3dcea-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3dcea-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="3dcea-121">Содержит состояние и результат одного [Операция GetSharingMetadata](getsharingmetadata-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="3dcea-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3dcea-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="3dcea-122">Remarks</span></span>

<span data-ttu-id="3dcea-123">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3dcea-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3dcea-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3dcea-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dcea-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3dcea-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3dcea-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3dcea-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3dcea-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3dcea-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3dcea-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3dcea-128">Validation File</span></span>  <br/> |<span data-ttu-id="3dcea-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3dcea-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3dcea-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3dcea-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3dcea-131">False</span><span class="sxs-lookup"><span data-stu-id="3dcea-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3dcea-132">См. также</span><span class="sxs-lookup"><span data-stu-id="3dcea-132">See also</span></span>

- [<span data-ttu-id="3dcea-133">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="3dcea-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="3dcea-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3dcea-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

