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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461270"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="308b2-103">енкриптедшаредфолдердатаколлектион</span><span class="sxs-lookup"><span data-stu-id="308b2-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="308b2-104">Элемент **енкриптедшаредфолдердатаколлектион** содержит коллекцию структур данных, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="308b2-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="308b2-105">**аррайофенкриптедшаредфолдердататипе**</span><span class="sxs-lookup"><span data-stu-id="308b2-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="308b2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="308b2-106">Attributes and elements</span></span>

<span data-ttu-id="308b2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="308b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="308b2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="308b2-108">Attributes</span></span>

<span data-ttu-id="308b2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="308b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="308b2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="308b2-110">Child elements</span></span>

|<span data-ttu-id="308b2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="308b2-111">**Element**</span></span>|<span data-ttu-id="308b2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="308b2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="308b2-113">енкриптедшаредфолдердата</span><span class="sxs-lookup"><span data-stu-id="308b2-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="308b2-114">Содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="308b2-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="308b2-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="308b2-115">Parent elements</span></span>

|<span data-ttu-id="308b2-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="308b2-116">**Element**</span></span>|<span data-ttu-id="308b2-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="308b2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="308b2-118">жетшарингметадатареспонсе</span><span class="sxs-lookup"><span data-stu-id="308b2-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="308b2-119">Определяет ответ на запрос [Операция GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="308b2-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="308b2-120">жетшарингметадатареспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="308b2-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="308b2-121">Содержит состояние и результат одного [Операция GetSharingMetadata](getsharingmetadata-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="308b2-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="308b2-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="308b2-122">Remarks</span></span>

<span data-ttu-id="308b2-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="308b2-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="308b2-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="308b2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="308b2-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="308b2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="308b2-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="308b2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="308b2-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="308b2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="308b2-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="308b2-128">Validation File</span></span>  <br/> |<span data-ttu-id="308b2-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="308b2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="308b2-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="308b2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="308b2-131">False</span><span class="sxs-lookup"><span data-stu-id="308b2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="308b2-132">См. также</span><span class="sxs-lookup"><span data-stu-id="308b2-132">See also</span></span>

- [<span data-ttu-id="308b2-133">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="308b2-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="308b2-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="308b2-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

