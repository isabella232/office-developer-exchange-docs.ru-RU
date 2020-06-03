---
title: Операция UpdateItem (Task)
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
ms.openlocfilehash: 0041af114d11fd9577037dd154e40b84e8483c35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459807"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="4015c-103">Операция UpdateItem (Task)</span><span class="sxs-lookup"><span data-stu-id="4015c-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="4015c-104">Операция UpdateItem используется для обновления свойств элемента задачи в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4015c-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4015c-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="4015c-105">Remarks</span></span>

<span data-ttu-id="4015c-106">Вы не можете отправлять запросы задач с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4015c-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="4015c-107">Веб-службы Exchange могут возвращать запросы задачи, созданные в Майкрософтofficeoutlook.</span><span class="sxs-lookup"><span data-stu-id="4015c-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="4015c-108">Если запрос задачи уже был отправлен, то запрос на обновление задачи возвратит ошибку.</span><span class="sxs-lookup"><span data-stu-id="4015c-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="4015c-109">Обновление текущего экземпляра повторяющейся задачи</span><span class="sxs-lookup"><span data-stu-id="4015c-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="4015c-110">Результат выполнения операции UpdateItem для повторяющихся задач отличается от результата операции UpdateItem для одной неповторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="4015c-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="4015c-111">Изменения, возникающие при возникновении повторяющейся задачи, приводят к созданию одноразовых задач при выполнении следующих обновлений:</span><span class="sxs-lookup"><span data-stu-id="4015c-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="4015c-112">Для свойства Status повторяющейся или повторяющейся задачи задано значение " **завершено**".</span><span class="sxs-lookup"><span data-stu-id="4015c-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="4015c-113">Изменена дата начала или Дата окончания повторяющейся задачи нонреженератинг.</span><span class="sxs-lookup"><span data-stu-id="4015c-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="4015c-114">Например, если запрос **UpdateItem** задает для выполнения повторяющейся задачи значение **true**, **упдатеитемреспонсе** будет включать новый идентификатор и чанжекэй, представляющие только что созданную одноразовую задачу.</span><span class="sxs-lookup"><span data-stu-id="4015c-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="4015c-115">Идентификатор, который был включен в запрос, по-прежнему действителен, а повторяющаяся задача, представленная этим идентификатором, была обновлена для представления следующего вхождения.</span><span class="sxs-lookup"><span data-stu-id="4015c-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="4015c-116">Чанжекэй, включенный в запрос, больше не является допустимым, так как повторяющаяся задача была обновлена.</span><span class="sxs-lookup"><span data-stu-id="4015c-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="4015c-117">Вы можете использовать [операцию GetItem](getitem-operation.md) , чтобы получить последние **чанжекэй** для повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="4015c-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="4015c-118">Для непериодических задач или последнего повторения повторяющейся задачи ответ UpdateItem возвращает тот же **идентификатор** , который был передан в него, и возвращает связанный обновленный **чанжекэй**.</span><span class="sxs-lookup"><span data-stu-id="4015c-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4015c-119">См. также</span><span class="sxs-lookup"><span data-stu-id="4015c-119">See also</span></span>



[<span data-ttu-id="4015c-120">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="4015c-120">UpdateItem operation</span></span>](updateitem-operation.md)

