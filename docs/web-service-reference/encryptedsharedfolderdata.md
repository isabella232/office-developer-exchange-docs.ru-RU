---
title: енкриптедшаредфолдердата
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
description: Элемент Енкриптедшаредфолдердата содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.
ms.openlocfilehash: 63966e95becaab4b3b1e54aa81f1b20a8b09dfd3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762333"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="05eb5-103">енкриптедшаредфолдердата</span><span class="sxs-lookup"><span data-stu-id="05eb5-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="05eb5-104">Элемент **енкриптедшаредфолдердата** содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="05eb5-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="05eb5-105">**енкриптедшаредфолдердататипе**</span><span class="sxs-lookup"><span data-stu-id="05eb5-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05eb5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="05eb5-106">Attributes and elements</span></span>

<span data-ttu-id="05eb5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="05eb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05eb5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="05eb5-108">Attributes</span></span>

<span data-ttu-id="05eb5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="05eb5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05eb5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="05eb5-110">Child elements</span></span>

|<span data-ttu-id="05eb5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="05eb5-111">**Element**</span></span>|<span data-ttu-id="05eb5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="05eb5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05eb5-113">Маркер</span><span class="sxs-lookup"><span data-stu-id="05eb5-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="05eb5-114">Содержит зашифрованные данные, представляющие маркер идентификации для общих данных.</span><span class="sxs-lookup"><span data-stu-id="05eb5-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="05eb5-115">Data</span><span class="sxs-lookup"><span data-stu-id="05eb5-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="05eb5-116">Содержит зашифрованные данные, представляющие общие данные.</span><span class="sxs-lookup"><span data-stu-id="05eb5-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05eb5-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="05eb5-117">Parent elements</span></span>

|<span data-ttu-id="05eb5-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="05eb5-118">**Element**</span></span>|<span data-ttu-id="05eb5-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="05eb5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05eb5-120">енкриптедшаредфолдердатаколлектион</span><span class="sxs-lookup"><span data-stu-id="05eb5-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="05eb5-121">Представляет коллекцию структур данных, которую клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="05eb5-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="05eb5-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="05eb5-122">Remarks</span></span>

<span data-ttu-id="05eb5-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="05eb5-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05eb5-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="05eb5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05eb5-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="05eb5-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05eb5-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="05eb5-126">Schema Name</span></span>  <br/> |<span data-ttu-id="05eb5-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="05eb5-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="05eb5-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="05eb5-128">Validation File</span></span>  <br/> |<span data-ttu-id="05eb5-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="05eb5-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05eb5-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="05eb5-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="05eb5-131">False</span><span class="sxs-lookup"><span data-stu-id="05eb5-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05eb5-132">См. также</span><span class="sxs-lookup"><span data-stu-id="05eb5-132">See also</span></span>

- [<span data-ttu-id="05eb5-133">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="05eb5-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="05eb5-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="05eb5-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

