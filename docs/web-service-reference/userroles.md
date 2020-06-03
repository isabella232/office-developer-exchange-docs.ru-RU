---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: Элемент UserRoles указывает роли пользователей, с которыми работает вызывающий пользователь, или пользователя, от которого работает партнерское приложение, необходимо применить к текущему вызову.
ms.openlocfilehash: 5155b82781321b16d1b58fdcaffe7b8cf2372717
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467132"
---
# <a name="userroles"></a><span data-ttu-id="39efa-103">UserRoles</span><span class="sxs-lookup"><span data-stu-id="39efa-103">UserRoles</span></span>

<span data-ttu-id="39efa-104">Элемент **UserRoles** указывает роли пользователей, с которыми работает вызывающий пользователь, или пользователя, от которого работает партнерское приложение, необходимо применить к текущему вызову.</span><span class="sxs-lookup"><span data-stu-id="39efa-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="39efa-105">**нонемптяррайофролетипе**</span><span class="sxs-lookup"><span data-stu-id="39efa-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39efa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="39efa-106">Attributes and elements</span></span>

<span data-ttu-id="39efa-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="39efa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39efa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="39efa-108">Attributes</span></span>

<span data-ttu-id="39efa-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="39efa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39efa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="39efa-110">Child elements</span></span>

[<span data-ttu-id="39efa-111">Role</span><span class="sxs-lookup"><span data-stu-id="39efa-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="39efa-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="39efa-112">Parent elements</span></span>

[<span data-ttu-id="39efa-113">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="39efa-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="39efa-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="39efa-114">Remarks</span></span>

<span data-ttu-id="39efa-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="39efa-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="39efa-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="39efa-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39efa-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="39efa-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39efa-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="39efa-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="39efa-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="39efa-119">Schema name</span></span>  <br/> |<span data-ttu-id="39efa-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="39efa-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="39efa-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="39efa-121">Validation file</span></span>  <br/> |<span data-ttu-id="39efa-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="39efa-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="39efa-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="39efa-123">Can be empty</span></span>  <br/> ||
   

