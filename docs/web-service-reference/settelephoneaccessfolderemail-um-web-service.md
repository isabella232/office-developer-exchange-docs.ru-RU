---
title: SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 90759da7-6dba-499e-b8c8-e44a016b3198
description: Элемент SetTelephoneAccessFolderEmail определяет запрос на установку папки электронной почты по умолчанию, из которой единая система обмена сообщениями будет читать сообщения по телефону.
ms.openlocfilehash: 806bdb1f0c7930a9e89555192aa32ad997716e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467321"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="14314-103">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="14314-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="14314-104">Элемент **SetTelephoneAccessFolderEmail** определяет запрос на установку папки электронной почты по умолчанию, из которой единая система обмена сообщениями будет читать сообщения по телефону.</span><span class="sxs-lookup"><span data-stu-id="14314-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="14314-105">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="14314-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="14314-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="14314-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14314-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="14314-107">Attributes and elements</span></span>

<span data-ttu-id="14314-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="14314-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14314-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="14314-109">Attributes</span></span>

<span data-ttu-id="14314-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14314-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14314-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="14314-111">Child elements</span></span>

|<span data-ttu-id="14314-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="14314-112">**Element**</span></span>|<span data-ttu-id="14314-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="14314-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14314-114">base64FolderId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="14314-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="14314-115">Идентификатор папки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="14314-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14314-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="14314-116">Parent elements</span></span>

<span data-ttu-id="14314-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14314-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="14314-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="14314-118">Text value</span></span>

<span data-ttu-id="14314-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14314-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14314-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="14314-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14314-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="14314-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="14314-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="14314-122">Schema Name</span></span>  <br/> |<span data-ttu-id="14314-123">Сообщения</span><span class="sxs-lookup"><span data-stu-id="14314-123">Messages</span></span>  <br/> |
|<span data-ttu-id="14314-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="14314-124">Validation File</span></span>  <br/> |<span data-ttu-id="14314-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="14314-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14314-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="14314-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="14314-127">False</span><span class="sxs-lookup"><span data-stu-id="14314-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14314-128">См. также</span><span class="sxs-lookup"><span data-stu-id="14314-128">See also</span></span>



[<span data-ttu-id="14314-129">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="14314-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

