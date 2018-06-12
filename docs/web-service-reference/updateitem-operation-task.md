---
title: Операция UpdateItem (задача)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: Операция UpdateItem используется для обновления свойств элемента задачи в хранилище Exchange.
ms.openlocfilehash: d6f966fa663300b476383a136d30cf611d6bfb9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840352"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="a7124-103">Операция UpdateItem (задача)</span><span class="sxs-lookup"><span data-stu-id="a7124-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="a7124-104">Операция UpdateItem используется для обновления свойств элемента задачи в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7124-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a7124-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="a7124-105">Remarks</span></span>

<span data-ttu-id="a7124-106">Веб-служб Exchange нельзя использовать для отправки запросов задач.</span><span class="sxs-lookup"><span data-stu-id="a7124-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="a7124-107">Веб-служб Exchange может вернуть запросы задач, созданных с MicrosoftOfficeOutlook.</span><span class="sxs-lookup"><span data-stu-id="a7124-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="a7124-108">Если уже был отправлен запрос задачи, запрос на обновление задачи возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="a7124-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="a7124-109">Обновление текущей копии повторяющейся задачи</span><span class="sxs-lookup"><span data-stu-id="a7124-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="a7124-110">Результат операции UpdateItem на повторяющиеся задачи отличается от результат операции UpdateItem single, неповторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="a7124-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="a7124-111">Изменение вхождения повторяющейся задачи приводит одноразовых задач, создаваемых при вносятся следующие обновления:</span><span class="sxs-lookup"><span data-stu-id="a7124-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="a7124-112">Свойство status восстанавливаемой или nonregenerating Повторяющаяся задача задано значение **завершено**.</span><span class="sxs-lookup"><span data-stu-id="a7124-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="a7124-113">Изменить дату начала или дату окончания nonregenerating Повторяющаяся задача.</span><span class="sxs-lookup"><span data-stu-id="a7124-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="a7124-114">Например если запрос **UpdateItem** устанавливает значение завершено повторяющейся задачи в **значение true**, **UpdateItemResponse** будет включать новый идентификатор и ChangeKey, которые представляют только что созданный одноразовых задач.</span><span class="sxs-lookup"><span data-stu-id="a7124-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="a7124-115">Идентификатор, который был включен в запрос действителен и повторяющейся задачи, представленного этот идентификатор Id был обновлен для представления следующее вхождение.</span><span class="sxs-lookup"><span data-stu-id="a7124-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="a7124-116">ChangeKey, который был включен в запросе больше не является допустимым, поскольку обновлена повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="a7124-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="a7124-117">[Операции GetItem](getitem-operation.md) можно использовать для получения последних **ChangeKey** для повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="a7124-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="a7124-118">Неповторяющейся задачи или последнего вхождения повторяющейся задачи ответа UpdateItem возвращает тот же **идентификатор** , переданным в него и возвращается связанный с ним обновленных **ChangeKey**.</span><span class="sxs-lookup"><span data-stu-id="a7124-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a7124-119">См. также</span><span class="sxs-lookup"><span data-stu-id="a7124-119">See also</span></span>



[<span data-ttu-id="a7124-120">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="a7124-120">UpdateItem operation</span></span>](updateitem-operation.md)

