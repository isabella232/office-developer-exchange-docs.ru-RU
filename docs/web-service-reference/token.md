---
title: Маркер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Token
api_type:
- schema
ms.assetid: 62b700e1-88c7-41ef-b431-d7af4a8b54a7
description: Элемент Token содержит зашифрованные данные, представляющие маркер идентификации для общих данных.
ms.openlocfilehash: c2e80082f9b4ecb96defdca8c5f0223a945661ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458910"
---
# <a name="token"></a><span data-ttu-id="fbce9-103">Маркер</span><span class="sxs-lookup"><span data-stu-id="fbce9-103">Token</span></span>

<span data-ttu-id="fbce9-104">Элемент **Token** содержит зашифрованные данные, представляющие маркер идентификации для общих данных.</span><span class="sxs-lookup"><span data-stu-id="fbce9-104">The **Token** element contains encrypted data that represents the identification token for the shared data.</span></span> 
  
```xml
<Token/>
```

 <span data-ttu-id="fbce9-105">**енкриптеддатаконтаинертипе**</span><span class="sxs-lookup"><span data-stu-id="fbce9-105">**EncryptedDataContainerType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbce9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fbce9-106">Attributes and elements</span></span>

<span data-ttu-id="fbce9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fbce9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbce9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fbce9-108">Attributes</span></span>

<span data-ttu-id="fbce9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fbce9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbce9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fbce9-110">Child elements</span></span>

<span data-ttu-id="fbce9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fbce9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fbce9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fbce9-112">Parent elements</span></span>

|<span data-ttu-id="fbce9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fbce9-113">**Element**</span></span>|<span data-ttu-id="fbce9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fbce9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbce9-115">енкриптедшаредфолдердата</span><span class="sxs-lookup"><span data-stu-id="fbce9-115">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="fbce9-116">Содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="fbce9-116">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fbce9-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="fbce9-117">Remarks</span></span>

<span data-ttu-id="fbce9-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fbce9-118">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbce9-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fbce9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbce9-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fbce9-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fbce9-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fbce9-121">Schema Name</span></span>  <br/> |<span data-ttu-id="fbce9-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fbce9-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="fbce9-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fbce9-123">Validation File</span></span>  <br/> |<span data-ttu-id="fbce9-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fbce9-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fbce9-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fbce9-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="fbce9-126">False</span><span class="sxs-lookup"><span data-stu-id="fbce9-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fbce9-127">См. также</span><span class="sxs-lookup"><span data-stu-id="fbce9-127">See also</span></span>



[<span data-ttu-id="fbce9-128">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="fbce9-128">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="fbce9-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fbce9-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

