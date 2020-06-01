---
title: енкриптедшаредфолдердатаколлектион
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
description: Элемент Енкриптедшаредфолдердатаколлектион содержит коллекцию структур данных, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.
ms.openlocfilehash: e8ed9221952892abda7b4eac62b16cdc4976c6e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461270"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="a354c-103">енкриптедшаредфолдердатаколлектион</span><span class="sxs-lookup"><span data-stu-id="a354c-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="a354c-104">Элемент **енкриптедшаредфолдердатаколлектион** содержит коллекцию структур данных, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="a354c-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="a354c-105">**аррайофенкриптедшаредфолдердататипе**</span><span class="sxs-lookup"><span data-stu-id="a354c-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a354c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a354c-106">Attributes and elements</span></span>

<span data-ttu-id="a354c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a354c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a354c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a354c-108">Attributes</span></span>

<span data-ttu-id="a354c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a354c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a354c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a354c-110">Child elements</span></span>

|<span data-ttu-id="a354c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a354c-111">**Element**</span></span>|<span data-ttu-id="a354c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a354c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a354c-113">енкриптедшаредфолдердата</span><span class="sxs-lookup"><span data-stu-id="a354c-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="a354c-114">Содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="a354c-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a354c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a354c-115">Parent elements</span></span>

|<span data-ttu-id="a354c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a354c-116">**Element**</span></span>|<span data-ttu-id="a354c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a354c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a354c-118">жетшарингметадатареспонсе</span><span class="sxs-lookup"><span data-stu-id="a354c-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="a354c-119">Определяет ответ на запрос [Операция GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a354c-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="a354c-120">жетшарингметадатареспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a354c-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="a354c-121">Содержит состояние и результат одного [Операция GetSharingMetadata](getsharingmetadata-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="a354c-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a354c-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="a354c-122">Remarks</span></span>

<span data-ttu-id="a354c-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a354c-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a354c-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a354c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a354c-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a354c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a354c-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a354c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a354c-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a354c-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a354c-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a354c-128">Validation File</span></span>  <br/> |<span data-ttu-id="a354c-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a354c-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a354c-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a354c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a354c-131">False</span><span class="sxs-lookup"><span data-stu-id="a354c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a354c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="a354c-132">See also</span></span>

- [<span data-ttu-id="a354c-133">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="a354c-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="a354c-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a354c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

