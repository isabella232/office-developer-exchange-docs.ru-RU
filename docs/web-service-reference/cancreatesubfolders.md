---
title: канкреатесубфолдерс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateSubFolders
api_type:
- schema
ms.assetid: 4404a1cc-6d3f-4996-9647-58a740e8f883
description: Элемент CanCreateSubFolders указывает, является ли пользователь имеет право на создание вложенных папок в папке. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d8e89c7a07ef1788717f5012840f5b8f79d319e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461599"
---
# <a name="cancreatesubfolders"></a><span data-ttu-id="929c5-104">канкреатесубфолдерс</span><span class="sxs-lookup"><span data-stu-id="929c5-104">CanCreateSubFolders</span></span>

<span data-ttu-id="929c5-p102">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **CanCreateSubFolders** указывает, является ли пользователь имеет право на создание вложенных папок в папке. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="929c5-p102">The **CanCreateSubFolders** element indicates whether a user has permission to create subfolders in a folder. This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateSubFolders/>
```

 <span data-ttu-id="929c5-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="929c5-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="929c5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="929c5-108">Attributes and elements</span></span>

<span data-ttu-id="929c5-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="929c5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="929c5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="929c5-110">Attributes</span></span>

<span data-ttu-id="929c5-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="929c5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="929c5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="929c5-112">Child elements</span></span>

<span data-ttu-id="929c5-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="929c5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="929c5-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="929c5-114">Parent elements</span></span>

|<span data-ttu-id="929c5-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="929c5-115">**Element**</span></span>|<span data-ttu-id="929c5-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="929c5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="929c5-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="929c5-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="929c5-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="929c5-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="929c5-120">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="929c5-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="929c5-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="929c5-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="929c5-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="929c5-123">Text value</span></span>

<span data-ttu-id="929c5-p105">Текстовое значение **true** указывает, что пользователь может создавать вложенные папки в папке. Значение **false** указывает, что пользователь не может создавать вложенные папки в папке.</span><span class="sxs-lookup"><span data-stu-id="929c5-p105">A text value of **true** indicates that the user can create subfolders in the folder. A value of **false** indicates that the user cannot create subfolders in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="929c5-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="929c5-126">Remarks</span></span>

<span data-ttu-id="929c5-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="929c5-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="929c5-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="929c5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="929c5-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="929c5-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="929c5-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="929c5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="929c5-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="929c5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="929c5-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="929c5-132">Validation File</span></span>  <br/> |<span data-ttu-id="929c5-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="929c5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="929c5-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="929c5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="929c5-135">False</span><span class="sxs-lookup"><span data-stu-id="929c5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="929c5-136">См. также</span><span class="sxs-lookup"><span data-stu-id="929c5-136">See also</span></span>



- [<span data-ttu-id="929c5-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="929c5-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="929c5-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="929c5-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

