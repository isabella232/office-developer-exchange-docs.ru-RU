---
title: IsContactPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsContactPhoto
api_type:
- schema
ms.assetid: ae36b5f9-a787-4863-9dbc-258ad724801d
description: Элемент IsContactPhoto указывает, является ли вложение файла изображение контакта.
ms.openlocfilehash: a015cd9bdb34ea9275952d5fe252a30cacf888ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833999"
---
# <a name="iscontactphoto"></a><span data-ttu-id="98848-103">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="98848-103">IsContactPhoto</span></span>

<span data-ttu-id="98848-104">Элемент **IsContactPhoto** указывает, является ли вложение файла изображение контакта.</span><span class="sxs-lookup"><span data-stu-id="98848-104">The **IsContactPhoto** element indicates whether the file attachment is a contact picture.</span></span> 
  
```xml
<IsContactPhoto>true or false</IsContactPhoto>
```

 <span data-ttu-id="98848-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="98848-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98848-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="98848-106">Attributes and elements</span></span>

<span data-ttu-id="98848-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="98848-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98848-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="98848-108">Attributes</span></span>

<span data-ttu-id="98848-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="98848-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98848-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="98848-110">Child elements</span></span>

<span data-ttu-id="98848-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="98848-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98848-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="98848-112">Parent elements</span></span>

|<span data-ttu-id="98848-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="98848-113">**Element**</span></span>|<span data-ttu-id="98848-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="98848-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98848-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="98848-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="98848-116">Представляет файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="98848-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98848-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="98848-117">Text value</span></span>

<span data-ttu-id="98848-118">Этот элемент может быть значение **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="98848-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="98848-119">Значение по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="98848-119">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98848-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="98848-120">Remarks</span></span>

<span data-ttu-id="98848-121">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="98848-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98848-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="98848-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98848-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="98848-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98848-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="98848-124">Schema Name</span></span>  <br/> |<span data-ttu-id="98848-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="98848-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="98848-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="98848-126">Validation File</span></span>  <br/> |<span data-ttu-id="98848-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="98848-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98848-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="98848-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="98848-129">False</span><span class="sxs-lookup"><span data-stu-id="98848-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98848-130">См. также</span><span class="sxs-lookup"><span data-stu-id="98848-130">See also</span></span>



- [<span data-ttu-id="98848-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="98848-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

