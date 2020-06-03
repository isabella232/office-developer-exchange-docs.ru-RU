---
title: GetPhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 5f4ee71c-bde0-4b0d-b426-0c24dfe67585
description: Элемент GetPhoneCallInformation указывает запрос на получение сведений о телефонном звонке.
ms.openlocfilehash: b835cd301b1c243e88034d1057026ef1305b9038
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530199"
---
# <a name="getphonecallinformation"></a><span data-ttu-id="932fd-103">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="932fd-103">GetPhoneCallInformation</span></span>

<span data-ttu-id="932fd-104">Элемент **GetPhoneCallInformation** указывает запрос на получение сведений о телефонном звонке.</span><span class="sxs-lookup"><span data-stu-id="932fd-104">The **GetPhoneCallInformation** element specifies a request to get telephone call information.</span></span> 
  
```xml
<GetPhoneCallInformation>
   <PhoneCallId/>
</GetPhoneCallInformation>
```

 <span data-ttu-id="932fd-105">**жетфонекаллинформатионтипе**</span><span class="sxs-lookup"><span data-stu-id="932fd-105">**GetPhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="932fd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="932fd-106">Attributes and elements</span></span>

<span data-ttu-id="932fd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="932fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="932fd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="932fd-108">Attributes</span></span>

<span data-ttu-id="932fd-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="932fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="932fd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="932fd-110">Child elements</span></span>

|<span data-ttu-id="932fd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="932fd-111">**Element**</span></span>|<span data-ttu-id="932fd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="932fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="932fd-113">фонекаллид</span><span class="sxs-lookup"><span data-stu-id="932fd-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="932fd-114">Задает идентификатор телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="932fd-114">Specifies the identifier of a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="932fd-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="932fd-115">Parent elements</span></span>

<span data-ttu-id="932fd-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="932fd-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="932fd-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="932fd-117">Text value</span></span>

<span data-ttu-id="932fd-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="932fd-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="932fd-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="932fd-119">Remarks</span></span>

<span data-ttu-id="932fd-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="932fd-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="932fd-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="932fd-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="932fd-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="932fd-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="932fd-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="932fd-123">Schema Name</span></span>  <br/> |<span data-ttu-id="932fd-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="932fd-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="932fd-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="932fd-125">Validation File</span></span>  <br/> |<span data-ttu-id="932fd-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="932fd-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="932fd-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="932fd-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="932fd-128">False</span><span class="sxs-lookup"><span data-stu-id="932fd-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="932fd-129">См. также</span><span class="sxs-lookup"><span data-stu-id="932fd-129">See also</span></span>



- [<span data-ttu-id="932fd-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="932fd-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

