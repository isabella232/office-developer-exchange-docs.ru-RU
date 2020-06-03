---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: Элемент GetSharingMetadata определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию. Этот элемент является базовым элементом для операции GetSharingMetadata.
ms.openlocfilehash: 406908e566d6d4249003b1a19a9ce79b8b328c4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530848"
---
# <a name="getsharingmetadata"></a><span data-ttu-id="9ce8d-104">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="9ce8d-104">GetSharingMetadata</span></span>

<span data-ttu-id="9ce8d-105">Элемент **GetSharingMetadata** определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-105">The **GetSharingMetadata** element defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span> <span data-ttu-id="9ce8d-106">Этот элемент является базовым элементом для [операции GetSharingMetadata](getsharingmetadata-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9ce8d-106">This element is the base element for the [GetSharingMetadata operation](getsharingmetadata-operation.md).</span></span>
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 <span data-ttu-id="9ce8d-107">**жетшарингметадататипе**</span><span class="sxs-lookup"><span data-stu-id="9ce8d-107">**GetSharingMetadataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ce8d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9ce8d-108">Attributes and elements</span></span>

<span data-ttu-id="9ce8d-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ce8d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9ce8d-110">Attributes</span></span>

<span data-ttu-id="9ce8d-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ce8d-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9ce8d-112">Child elements</span></span>

|<span data-ttu-id="9ce8d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9ce8d-113">**Element**</span></span>|<span data-ttu-id="9ce8d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9ce8d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ce8d-115">идоффолдертошаре</span><span class="sxs-lookup"><span data-stu-id="9ce8d-115">IdOfFolderToShare</span></span>](idoffoldertoshare.md) <br/> |<span data-ttu-id="9ce8d-116">Представляет идентификатор папки на сервере, к которой будет предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-116">Represents the identifier of the folder on the server that will be shared.</span></span> <span data-ttu-id="9ce8d-117">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="9ce8d-118">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="9ce8d-118">SenderSmtpAddress</span></span>](sendersmtpaddress.md) <br/> |<span data-ttu-id="9ce8d-119">Представляет SMTP-адрес электронной почты, соответствующий почтовому ящику, содержащему папку, определяемую элементом [идоффолдертошаре](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="9ce8d-119">Represents the SMTP email address that corresponds to the mailbox that contains the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="9ce8d-120">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="9ce8d-121">Получатели (Аррайофсмтпаддресстипе)</span><span class="sxs-lookup"><span data-stu-id="9ce8d-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="9ce8d-122">Представляет SMTP-адреса электронной почты одного или нескольких сущностей, которым будет предоставлен доступ к данным в папке, указанной с помощью элемента [идоффолдертошаре](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="9ce8d-122">Represents the SMTP email addresses of one or more entities that will be granted access to the data in the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="9ce8d-123">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-123">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ce8d-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9ce8d-124">Parent elements</span></span>

<span data-ttu-id="9ce8d-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9ce8d-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ce8d-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9ce8d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ce8d-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9ce8d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9ce8d-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9ce8d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9ce8d-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9ce8d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9ce8d-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9ce8d-130">Validation File</span></span>  <br/> |<span data-ttu-id="9ce8d-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9ce8d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ce8d-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9ce8d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ce8d-133">False</span><span class="sxs-lookup"><span data-stu-id="9ce8d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ce8d-134">См. также</span><span class="sxs-lookup"><span data-stu-id="9ce8d-134">See also</span></span>



[<span data-ttu-id="9ce8d-135">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="9ce8d-135">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="9ce8d-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9ce8d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

