---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: Элемент EncryptedSharedFolderData содержит зашифрованные данные, клиента можно использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.
ms.openlocfilehash: 63966e95becaab4b3b1e54aa81f1b20a8b09dfd3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762333"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="56a0f-103">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="56a0f-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="56a0f-104">Элемент **EncryptedSharedFolderData** содержит зашифрованные данные, клиента можно использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.</span><span class="sxs-lookup"><span data-stu-id="56a0f-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="56a0f-105">**EncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="56a0f-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56a0f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="56a0f-106">Attributes and elements</span></span>

<span data-ttu-id="56a0f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="56a0f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56a0f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="56a0f-108">Attributes</span></span>

<span data-ttu-id="56a0f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="56a0f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56a0f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="56a0f-110">Child elements</span></span>

|<span data-ttu-id="56a0f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="56a0f-111">**Element**</span></span>|<span data-ttu-id="56a0f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="56a0f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a0f-113">Маркер</span><span class="sxs-lookup"><span data-stu-id="56a0f-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="56a0f-114">Содержит зашифрованные данные, который представляет маркер идентификации для общих данных.</span><span class="sxs-lookup"><span data-stu-id="56a0f-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="56a0f-115">Данные</span><span class="sxs-lookup"><span data-stu-id="56a0f-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="56a0f-116">Содержит зашифрованные данные, представляющий общих данных.</span><span class="sxs-lookup"><span data-stu-id="56a0f-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56a0f-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="56a0f-117">Parent elements</span></span>

|<span data-ttu-id="56a0f-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="56a0f-118">**Element**</span></span>|<span data-ttu-id="56a0f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="56a0f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a0f-120">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="56a0f-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="56a0f-121">Представляет коллекцию структур данных, которые клиент может использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.</span><span class="sxs-lookup"><span data-stu-id="56a0f-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="56a0f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="56a0f-122">Remarks</span></span>

<span data-ttu-id="56a0f-123">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="56a0f-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56a0f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="56a0f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56a0f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="56a0f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56a0f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="56a0f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="56a0f-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="56a0f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="56a0f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="56a0f-128">Validation File</span></span>  <br/> |<span data-ttu-id="56a0f-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="56a0f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56a0f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="56a0f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="56a0f-131">False</span><span class="sxs-lookup"><span data-stu-id="56a0f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56a0f-132">См. также</span><span class="sxs-lookup"><span data-stu-id="56a0f-132">See also</span></span>

- [<span data-ttu-id="56a0f-133">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="56a0f-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="56a0f-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="56a0f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

