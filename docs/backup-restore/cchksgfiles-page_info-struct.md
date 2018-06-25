---
title: Структура CChkSGFiles.PAGE_INFO
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
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761859"
---
# <a name="cchksgfilespageinfo-struct"></a><span data-ttu-id="485ff-103">Структура CChkSGFiles.PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="485ff-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="485ff-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="485ff-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="485ff-105">Содержит сведения о странице базы данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="485ff-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="485ff-106">Эта структура используется с функцией **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="485ff-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
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

## <a name="members"></a><span data-ttu-id="485ff-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="485ff-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="485ff-108">ulPgNo</span><span class="sxs-lookup"><span data-stu-id="485ff-108">ulPgNo</span></span>
  
<span data-ttu-id="485ff-109">Длинное целое без знака.</span><span class="sxs-lookup"><span data-stu-id="485ff-109">Unsigned Long.</span></span> <span data-ttu-id="485ff-110">Число страниц базы данных для проверки логической страницы.</span><span class="sxs-lookup"><span data-stu-id="485ff-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="485ff-111">Это значение должно быть задано до вызова метода **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="485ff-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="485ff-112">Если приложение читает файл на основании файла смещения и поэтому необходимо сопоставить смещения этих файлов логические номера страниц, вы найдете метод **PgnoFromFileOffset** полезен для определения значения для этого поля.</span><span class="sxs-lookup"><span data-stu-id="485ff-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="485ff-113">**ErrCheckDbPages** не изменяет это значение.</span><span class="sxs-lookup"><span data-stu-id="485ff-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="485ff-114">fPageIsInitialized</span><span class="sxs-lookup"><span data-stu-id="485ff-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="485ff-115">Логическое значение.</span><span class="sxs-lookup"><span data-stu-id="485ff-115">Boolean.</span></span> <span data-ttu-id="485ff-116">Значение TRUE означает, что страница база данных содержит данные.</span><span class="sxs-lookup"><span data-stu-id="485ff-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="485ff-117">Значение FALSE указывает, что страница содержит только нули.</span><span class="sxs-lookup"><span data-stu-id="485ff-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="485ff-118">Это значение устанавливается **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="485ff-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="485ff-119">fCorrectableError</span><span class="sxs-lookup"><span data-stu-id="485ff-119">fCorrectableError</span></span>
  
<span data-ttu-id="485ff-120">Логическое значение.</span><span class="sxs-lookup"><span data-stu-id="485ff-120">Boolean.</span></span> <span data-ttu-id="485ff-121">Значение TRUE указывает, что произошла ошибка контрольной суммы, обнаруженных в странице базы данных, но, что это Исправимая ошибка.</span><span class="sxs-lookup"><span data-stu-id="485ff-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="485ff-122">Это значение устанавливается **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="485ff-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="485ff-123">checksumActual</span><span class="sxs-lookup"><span data-stu-id="485ff-123">checksumActual</span></span>
  
<span data-ttu-id="485ff-124">Неподписанные 64-разрядное целое число.</span><span class="sxs-lookup"><span data-stu-id="485ff-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="485ff-125">Указывает значение контрольной суммой, хранящиеся в базе данных для этой логической страницы.</span><span class="sxs-lookup"><span data-stu-id="485ff-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="485ff-126">Это значение устанавливается **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="485ff-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="485ff-127">checksumExpected</span><span class="sxs-lookup"><span data-stu-id="485ff-127">checksumExpected</span></span>
  
<span data-ttu-id="485ff-128">Неподписанные 64-разрядное целое число.</span><span class="sxs-lookup"><span data-stu-id="485ff-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="485ff-129">Это значение ожидаемой, вычисленные для страницы базы данных; оно установлено по **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="485ff-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="485ff-130">Если это значение отличается от, хранящиеся на странице базы данных (то есть, значение, возвращаемое в **checksumActual**), **ErrCheckDbPages** появится сообщение о том, что на этой странице базы данных обнаружены ошибки.</span><span class="sxs-lookup"><span data-stu-id="485ff-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="485ff-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="485ff-131">dbTime</span></span>
  
<span data-ttu-id="485ff-132">Неподписанные 64-разрядное целое число.</span><span class="sxs-lookup"><span data-stu-id="485ff-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="485ff-133">**ErrCheckDbPages** устанавливает этот член метка времени на странице базы данных.</span><span class="sxs-lookup"><span data-stu-id="485ff-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="485ff-134">checksumPageStructure</span><span class="sxs-lookup"><span data-stu-id="485ff-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="485ff-135">Целое 64-bt.</span><span class="sxs-lookup"><span data-stu-id="485ff-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="485ff-136">**ErrCheckDbPages** задает этот член со значением вычисляемые содержимого страницы, за исключением данных, который не требуется, при определении эквивалентности логической страницы.</span><span class="sxs-lookup"><span data-stu-id="485ff-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="485ff-137">Например нет необходимости необходимо рассмотреть значений данных в место неиспользуемых базы данных.</span><span class="sxs-lookup"><span data-stu-id="485ff-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="485ff-138">Этот член допустимо только в том случае, если значения **checksumActual** и **checksumExpected** равны друг с другом.</span><span class="sxs-lookup"><span data-stu-id="485ff-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="485ff-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="485ff-139">ulFlags</span></span>
  
<span data-ttu-id="485ff-140">Неподписанные 64-разрядное целое число.</span><span class="sxs-lookup"><span data-stu-id="485ff-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="485ff-141">Зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="485ff-141">Reserved for future use.</span></span> <span data-ttu-id="485ff-142">Значение в этом поле должно иметь значение нуль (0) до вызова метода **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="485ff-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="485ff-143">Замечания</span><span class="sxs-lookup"><span data-stu-id="485ff-143">Remarks</span></span>

<span data-ttu-id="485ff-144">При вызове функции **ErrCheckDbPages** , параметр **rgPageInfo** представляет собой массив из **Страница\_INFO** структуры.</span><span class="sxs-lookup"><span data-stu-id="485ff-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="485ff-145">Должно быть одно **Страница\_INFO** структуры для каждой страницы базы данных для проверки.</span><span class="sxs-lookup"><span data-stu-id="485ff-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="485ff-146">Приложение необходимо присвоить член **ulPgno** правильное значение и необходимо также установить член **ulFlags** в нуль (0) до вызова метода **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="485ff-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="485ff-147">Требования</span><span class="sxs-lookup"><span data-stu-id="485ff-147">Requirements</span></span>

<span data-ttu-id="485ff-148">Exchange Server 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="485ff-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="485ff-149">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="485ff-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

