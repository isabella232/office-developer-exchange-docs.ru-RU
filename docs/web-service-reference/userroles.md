---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: Элемент UserRoles указывает ролей пользователей, вызывающего пользователя или на уровне пользователя, вызывающий партнерское приложение используется в качестве, требуется применить текущий звонок.
ms.openlocfilehash: 19dc1a7e00decb9141326b53b650d72101013c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840438"
---
# <a name="userroles"></a><span data-ttu-id="e56ee-103">UserRoles</span><span class="sxs-lookup"><span data-stu-id="e56ee-103">UserRoles</span></span>

<span data-ttu-id="e56ee-104">Элемент **UserRoles** указывает ролей пользователей, вызывающего пользователя или на уровне пользователя, вызывающий партнерское приложение используется в качестве, требуется применить текущий звонок.</span><span class="sxs-lookup"><span data-stu-id="e56ee-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="e56ee-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="e56ee-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e56ee-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e56ee-106">Attributes and elements</span></span>

<span data-ttu-id="e56ee-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e56ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e56ee-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e56ee-108">Attributes</span></span>

<span data-ttu-id="e56ee-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e56ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e56ee-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e56ee-110">Child elements</span></span>

[<span data-ttu-id="e56ee-111">Роль</span><span class="sxs-lookup"><span data-stu-id="e56ee-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="e56ee-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e56ee-112">Parent elements</span></span>

[<span data-ttu-id="e56ee-113">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="e56ee-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="e56ee-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="e56ee-114">Remarks</span></span>

<span data-ttu-id="e56ee-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e56ee-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e56ee-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e56ee-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e56ee-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e56ee-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e56ee-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e56ee-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e56ee-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e56ee-119">Schema name</span></span>  <br/> |<span data-ttu-id="e56ee-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e56ee-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="e56ee-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e56ee-121">Validation file</span></span>  <br/> |<span data-ttu-id="e56ee-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e56ee-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e56ee-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e56ee-123">Can be empty</span></span>  <br/> ||
   

