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
ms.openlocfilehash: 52e91eaf1ded31602b11e50c1b62159f72c101cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530665"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="7a961-103">енкриптедшаредфолдердата</span><span class="sxs-lookup"><span data-stu-id="7a961-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="7a961-104">Элемент **енкриптедшаредфолдердата** содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="7a961-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="7a961-105">**енкриптедшаредфолдердататипе**</span><span class="sxs-lookup"><span data-stu-id="7a961-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a961-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a961-106">Attributes and elements</span></span>

<span data-ttu-id="7a961-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7a961-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a961-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a961-108">Attributes</span></span>

<span data-ttu-id="7a961-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7a961-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a961-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a961-110">Child elements</span></span>

|<span data-ttu-id="7a961-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a961-111">**Element**</span></span>|<span data-ttu-id="7a961-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a961-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a961-113">Маркер</span><span class="sxs-lookup"><span data-stu-id="7a961-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="7a961-114">Содержит зашифрованные данные, представляющие маркер идентификации для общих данных.</span><span class="sxs-lookup"><span data-stu-id="7a961-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="7a961-115">Data</span><span class="sxs-lookup"><span data-stu-id="7a961-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="7a961-116">Содержит зашифрованные данные, представляющие общие данные.</span><span class="sxs-lookup"><span data-stu-id="7a961-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a961-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a961-117">Parent elements</span></span>

|<span data-ttu-id="7a961-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a961-118">**Element**</span></span>|<span data-ttu-id="7a961-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a961-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a961-120">енкриптедшаредфолдердатаколлектион</span><span class="sxs-lookup"><span data-stu-id="7a961-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="7a961-121">Представляет коллекцию структур данных, которую клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="7a961-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a961-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="7a961-122">Remarks</span></span>

<span data-ttu-id="7a961-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7a961-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a961-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a961-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a961-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a961-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a961-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a961-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7a961-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7a961-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a961-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a961-128">Validation File</span></span>  <br/> |<span data-ttu-id="7a961-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7a961-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a961-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a961-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a961-131">False</span><span class="sxs-lookup"><span data-stu-id="7a961-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a961-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7a961-132">See also</span></span>

- [<span data-ttu-id="7a961-133">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="7a961-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="7a961-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7a961-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

