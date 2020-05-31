---
title: Структура функция cchksgfiles. PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761859"
---
# <a name="cchksgfilespage_info-struct"></a><span data-ttu-id="5d5fb-103">Структура функция cchksgfiles. PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="5d5fb-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="5d5fb-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d5fb-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="5d5fb-105">Содержит сведения для страницы базы данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="5d5fb-106">Эта структура используется с функцией **еррчеккдбпажес** .</span><span class="sxs-lookup"><span data-stu-id="5d5fb-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a><span data-ttu-id="5d5fb-107">"Участники"</span><span class="sxs-lookup"><span data-stu-id="5d5fb-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="5d5fb-108">улпгно</span><span class="sxs-lookup"><span data-stu-id="5d5fb-108">ulPgNo</span></span>
  
<span data-ttu-id="5d5fb-109">Длинное целое без знака.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-109">Unsigned Long.</span></span> <span data-ttu-id="5d5fb-110">Логический номер страницы базы данных, которую необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="5d5fb-111">Это значение должно быть задано до вызова **еррчеккдбпажес**.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="5d5fb-112">Если приложение читает файл на основе смещений файлов, и поэтому необходимо сопоставить эти смещения файлов с логическими номерами страниц, можно найти метод **пгнофромфилеоффсет** , который полезен для определения значения для этого поля.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="5d5fb-113">**Еррчеккдбпажес** не изменяет это значение.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="5d5fb-114">фпажеисинитиализед</span><span class="sxs-lookup"><span data-stu-id="5d5fb-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="5d5fb-115">Логического.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-115">Boolean.</span></span> <span data-ttu-id="5d5fb-116">Значение TRUE указывает на то, что страница базы данных содержит данные.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="5d5fb-117">Значение FALSE указывает на то, что страница содержит только нули.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="5d5fb-118">**Еррчеккдбпажес** задает это значение.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="5d5fb-119">фкорректаблиррор</span><span class="sxs-lookup"><span data-stu-id="5d5fb-119">fCorrectableError</span></span>
  
<span data-ttu-id="5d5fb-120">Логического.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-120">Boolean.</span></span> <span data-ttu-id="5d5fb-121">Значение TRUE указывает на то, что на странице базы данных обнаружено несоответствие контрольной суммы, но это устранимая ошибка.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="5d5fb-122">**Еррчеккдбпажес** задает это значение.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="5d5fb-123">чекксумактуал</span><span class="sxs-lookup"><span data-stu-id="5d5fb-123">checksumActual</span></span>
  
<span data-ttu-id="5d5fb-124">64 — разрядное целое число без знака.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="5d5fb-125">Указывает значение контрольной суммы, хранящегося в базе данных для этой логической страницы.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="5d5fb-126">**Еррчеккдбпажес** задает это значение.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="5d5fb-127">чекксумекспектед</span><span class="sxs-lookup"><span data-stu-id="5d5fb-127">checksumExpected</span></span>
  
<span data-ttu-id="5d5fb-128">64 — разрядное целое число без знака.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="5d5fb-129">Это ожидаемое значение контрольной суммы, вычисляемое для страницы базы данных; Он задается с помощью **еррчеккдбпажес**.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="5d5fb-130">Если это значение отличается от того, которое хранится на странице базы данных (то есть значение, возвращаемое в **чекксумактуал**), **еррчеккдбпажес** указывает на то, что на этой странице базы данных обнаружена ошибка.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="5d5fb-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="5d5fb-131">dbTime</span></span>
  
<span data-ttu-id="5d5fb-132">64 — разрядное целое число без знака.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="5d5fb-133">**Еррчеккдбпажес** задает для этого элемента значение timestamp на странице базы данных.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="5d5fb-134">чекксумпажеструктуре</span><span class="sxs-lookup"><span data-stu-id="5d5fb-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="5d5fb-135">Целое число без знака 64 — BT.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="5d5fb-136">**Еррчеккдбпажес** задает для этого элемента вычисленное значение контрольной суммы содержимого страницы без ненужных данных при определении эквивалентности логической страницы.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="5d5fb-137">Например, не требуется учитывать значения данных в неиспользуемом пространстве страниц базы данных.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="5d5fb-138">Этот элемент является допустимым только в том случае, если значения **чекксумактуал** и **чекксумекспектед** равны друг другу.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="5d5fb-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="5d5fb-139">ulFlags</span></span>
  
<span data-ttu-id="5d5fb-140">64 — разрядное целое число без знака.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="5d5fb-141">Зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-141">Reserved for future use.</span></span> <span data-ttu-id="5d5fb-142">Перед вызовом метода **еррчеккдбпажес**необходимо задать для этого поля значение 0 (ноль).</span><span class="sxs-lookup"><span data-stu-id="5d5fb-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="5d5fb-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="5d5fb-143">Remarks</span></span>

<span data-ttu-id="5d5fb-144">При вызове функции **еррчеккдбпажес** параметр **ргпажеинфо** является массивом структур **сведений о странице\_** .</span><span class="sxs-lookup"><span data-stu-id="5d5fb-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="5d5fb-145">Для проверки каждой страницы базы данных должна быть одна структура **сведений о странице\_** .</span><span class="sxs-lookup"><span data-stu-id="5d5fb-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="5d5fb-146">Приложение должно присвоить элементу **улпгно** правильное значение, а также установить для члена **ulFlags** значение 0 (ноль) перед вызовом **еррчеккдбпажес**.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="5d5fb-147">Requirements</span><span class="sxs-lookup"><span data-stu-id="5d5fb-147">Requirements</span></span>

<span data-ttu-id="5d5fb-148">Exchange Server 2013 включает в себя только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="5d5fb-149">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="5d5fb-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

