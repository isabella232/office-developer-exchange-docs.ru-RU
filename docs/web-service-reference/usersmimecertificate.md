---
title: UserSMIMECertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 66e6b4ba-368d-4469-bd47-e59441b7d64d
description: Элемент UserSMIMECertificate содержит значение, которое кодирует сертификат SMIME контакта.
ms.openlocfilehash: 7e2dbc6a9c8b04758ba99db036e237d8837850aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467657"
---
# <a name="usersmimecertificate"></a><span data-ttu-id="179bc-103">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="179bc-103">UserSMIMECertificate</span></span>

<span data-ttu-id="179bc-104">Элемент **UserSMIMECertificate** содержит значение, которое КОДИРУЕТ сертификат SMIME контакта.</span><span class="sxs-lookup"><span data-stu-id="179bc-104">The **UserSMIMECertificate** element contains a value that encodes a contact's SMIME certificate.</span></span> 
  
```XML
<UserSMIMECertificate/>
```

 <span data-ttu-id="179bc-105">**аррайофбинаритипе**</span><span class="sxs-lookup"><span data-stu-id="179bc-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="179bc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="179bc-106">Attributes and elements</span></span>

<span data-ttu-id="179bc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="179bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="179bc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="179bc-108">Attributes</span></span>

<span data-ttu-id="179bc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="179bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="179bc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="179bc-110">Child elements</span></span>

|<span data-ttu-id="179bc-111">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="179bc-111">**Element name**</span></span>|<span data-ttu-id="179bc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="179bc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="179bc-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="179bc-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="179bc-114">Содержит значение, закодированное в формате Base64.</span><span class="sxs-lookup"><span data-stu-id="179bc-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="179bc-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="179bc-115">Parent elements</span></span>

|<span data-ttu-id="179bc-116">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="179bc-116">**Element name**</span></span>|<span data-ttu-id="179bc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="179bc-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="179bc-118">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="179bc-118">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="179bc-119">Представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="179bc-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="179bc-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="179bc-120">Text value</span></span>

<span data-ttu-id="179bc-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="179bc-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="179bc-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="179bc-122">Remarks</span></span>

<span data-ttu-id="179bc-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="179bc-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="179bc-124">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="179bc-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="179bc-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="179bc-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="179bc-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="179bc-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="179bc-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="179bc-127">Schema name</span></span>  <br/> |<span data-ttu-id="179bc-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="179bc-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="179bc-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="179bc-129">Validation file</span></span>  <br/> |<span data-ttu-id="179bc-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="179bc-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="179bc-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="179bc-131">Can be empty</span></span>  <br/> |<span data-ttu-id="179bc-132">False</span><span class="sxs-lookup"><span data-stu-id="179bc-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="179bc-133">См. также</span><span class="sxs-lookup"><span data-stu-id="179bc-133">See also</span></span>



- [<span data-ttu-id="179bc-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="179bc-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="179bc-135">Создание контактов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="179bc-135">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

