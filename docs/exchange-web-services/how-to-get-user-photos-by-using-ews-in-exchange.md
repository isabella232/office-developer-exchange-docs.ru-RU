---
title: Получение фотографий пользователей с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Узнайте, как получить фотографии пользователей, связанные с почтовым ящиком или контактом, с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 14f2bc6bef1ce3c3529f03e213e3ada7c45a5a71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455788"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a><span data-ttu-id="d0d82-103">Получение фотографий пользователей с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d0d82-103">Get user photos by using EWS in Exchange</span></span>

<span data-ttu-id="d0d82-104">Узнайте, как получить фотографии пользователей, связанные с почтовым ящиком или контактом, с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0d82-104">Learn how to get user photos that are associated with a mailbox or contact by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="d0d82-105">Удобно добавлять лицо в имя.</span><span class="sxs-lookup"><span data-stu-id="d0d82-105">It's nice to put a face to a name.</span></span> <span data-ttu-id="d0d82-106">Если пользователям требуется добавлять имена в грани, приложение может запросить изображение, как правило, фотографию, из Exchange, который представляет учетную запись электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d0d82-106">If your users like to put names to faces, your application can request an image, typically a photo, from Exchange that represents an email account.</span></span> <span data-ttu-id="d0d82-107">Вы можете получить фотографию пользователя, сохраненную на сервере Exchange Server для почтового ящика, или получить фотографию контакта из контактов, хранящихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d0d82-107">You can get a user photo stored on an Exchange server for a mailbox, or you can get a contact photo from contacts stored in your mailbox.</span></span>
  
<span data-ttu-id="d0d82-108">Вы можете использовать несколько различных технологий для получения фотографий из почтовых ящиков или доменных служб Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="d0d82-108">You can use several different technologies to get photos from mailboxes or Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="d0d82-109">Лучший способ получить фотографию зависит от типа контакта, с которого вы хотите получить фотографию.</span><span class="sxs-lookup"><span data-stu-id="d0d82-109">The best way to get a photo depends on the type of contact that you want to get a photo from.</span></span> 
  
<span data-ttu-id="d0d82-110">**Таблица 1. Технологии, используемые для получения фотографий пользователей на основе типа контакта**</span><span class="sxs-lookup"><span data-stu-id="d0d82-110">**Table 1. Technologies to use to get user photos based on contact type**</span></span>

|<span data-ttu-id="d0d82-111">**Тип контакта**</span><span class="sxs-lookup"><span data-stu-id="d0d82-111">**Contact type**</span></span>|<span data-ttu-id="d0d82-112">**Используемые технологии**</span><span class="sxs-lookup"><span data-stu-id="d0d82-112">**Technologies to use**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d0d82-113">Фотография пользователя почтового ящика</span><span class="sxs-lookup"><span data-stu-id="d0d82-113">Mailbox user photo</span></span>  <br/> |[<span data-ttu-id="d0d82-114">Получение фотографии пользователя почтового ящика с помощью REST</span><span class="sxs-lookup"><span data-stu-id="d0d82-114">Get a mailbox user photo by using REST</span></span>](#bk_REST)<br/><br/> [<span data-ttu-id="d0d82-115">Получение фотографии пользователя с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="d0d82-115">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |
|<span data-ttu-id="d0d82-116">Фотография пользователя контакта</span><span class="sxs-lookup"><span data-stu-id="d0d82-116">Contact user photo</span></span>  <br/> |[<span data-ttu-id="d0d82-117">Получение фотографии пользователя контакта с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="d0d82-117">Get a contact user photo by using EWS Managed API</span></span>](#bk_EWSMA)<br/><br/> [<span data-ttu-id="d0d82-118">Получение фотографии пользователя с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="d0d82-118">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |

<span data-ttu-id="d0d82-119"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="d0d82-119"><a name="bk_REST"> </a></span></span>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a><span data-ttu-id="d0d82-120">Получение фотографии пользователя почтового ящика с помощью REST</span><span class="sxs-lookup"><span data-stu-id="d0d82-120">Get a mailbox user photo by using REST</span></span>

<span data-ttu-id="d0d82-121">Вы можете запросить фотографии пользователей с сервера Exchange, используя стандартный запрос **Get** HTTPS.</span><span class="sxs-lookup"><span data-stu-id="d0d82-121">You can request user photos from an Exchange server by using a standard HTTPS **GET** request.</span></span> <span data-ttu-id="d0d82-122">В запросе укажите адрес учетной записи электронной почты и код размера для изображения, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="d0d82-122">In the request, specify the email account address and a size code for the image, as shown in the following example.</span></span> 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

<span data-ttu-id="d0d82-123">Используйте операцию [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) службы автообнаружения для получения параметра **екстерналевсурл** , который содержит URL-адрес конечной точки веб-служб Exchange (EWS), и расположение обработчика HTTP- **сообщений Exchange. asmx** , который возвращает фотографии пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0d82-123">Use the Autodiscover service [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) operation to retrieve the **ExternalEwsUrl** setting, which contains the URL of the Exchange Web Services (EWS) endpoint and the location of the **Exchange.asmx** HTTP handler that returns the user photos.</span></span> 
  
<span data-ttu-id="d0d82-124">Каждый код размера указывает высоту и ширину изображения в пикселях.</span><span class="sxs-lookup"><span data-stu-id="d0d82-124">Each size code indicates the height and width of the image in pixels.</span></span> <span data-ttu-id="d0d82-125">Например, код размера **HR48x48** возвращает изображение размером 48 пикселей в высоту, равное 48 x ширина.</span><span class="sxs-lookup"><span data-stu-id="d0d82-125">For example, the size code **HR48x48** returns an image that is 48 pixels high by 48 pixels wide.</span></span> <span data-ttu-id="d0d82-126">Возможные значения параметра кода размера совпадают с возможными значениями для элемента [сизерекуестед](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d0d82-126">The possible values for the size code parameter are the same as the possible values for the [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="d0d82-127">Если запрос указывает недоступный размер, будет возвращена самая большая доступная фотография.</span><span class="sxs-lookup"><span data-stu-id="d0d82-127">If the request specifies a size that is not available, the largest available photo will be returned.</span></span> <span data-ttu-id="d0d82-128">Если на сервере Exchange не хранится фотография, будет возвращено эскизное изображение, хранящееся в доменных СЛУЖБах Active Directory для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d0d82-128">If no photo is stored on the Exchange server, the thumbnail image stored in AD DS for the account will be returned.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d0d82-129">Код размера **HR48x48** всегда возвращает изображение ЭСКИЗА AD DS, если оно доступно.</span><span class="sxs-lookup"><span data-stu-id="d0d82-129">The **HR48x48** size code always returns the AD DS thumbnail image if it is available.</span></span> 
  
<span data-ttu-id="d0d82-130">В приведенном ниже примере показано, как можно использовать запрос GET для получения фотографии пользователя для Ольга и сохранения его на локальном компьютере.</span><span class="sxs-lookup"><span data-stu-id="d0d82-130">The following example shows how you can use the GET request to retrieve the user photo for Sadie and save it to your local computer.</span></span>
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

<span data-ttu-id="d0d82-131">Запрос возвратит HTTP-ответ.</span><span class="sxs-lookup"><span data-stu-id="d0d82-131">The request will return an HTTP response.</span></span> 
  
<span data-ttu-id="d0d82-132">**Таблица 2. Коды отклика для запроса GetUserPhoto**</span><span class="sxs-lookup"><span data-stu-id="d0d82-132">**Table 2. Response codes for a GetUserPhoto request**</span></span>

|<span data-ttu-id="d0d82-133">**Response code** (Код ответа)</span><span class="sxs-lookup"><span data-stu-id="d0d82-133">**Response code**</span></span>|<span data-ttu-id="d0d82-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0d82-134">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d0d82-135">200</span><span class="sxs-lookup"><span data-stu-id="d0d82-135">200</span></span>  <br/> |<span data-ttu-id="d0d82-136">Для указанной учетной записи электронной почты доступен образ, а в ответе присутствует двоичный образ.</span><span class="sxs-lookup"><span data-stu-id="d0d82-136">An image is available for the specified email account and the binary image is contained in the response.</span></span>  <br/> |
|<span data-ttu-id="d0d82-137">304</span><span class="sxs-lookup"><span data-stu-id="d0d82-137">304</span></span>  <br/> |<span data-ttu-id="d0d82-138">Изображение не изменилось со времени последнего возврата **ETag** в приложение.</span><span class="sxs-lookup"><span data-stu-id="d0d82-138">The image has not changed since the last time the **ETag** was returned to the application.</span></span>  <br/> |
|<span data-ttu-id="d0d82-139">404</span><span class="sxs-lookup"><span data-stu-id="d0d82-139">404</span></span>  <br/> |<span data-ttu-id="d0d82-140">Нет доступных изображений для указанной учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d0d82-140">No image is available for the specified email account.</span></span>  <br/> |

<span data-ttu-id="d0d82-141"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="d0d82-141"><a name="bk_REST"> </a></span></span>

## <a name="cache-user-photos"></a><span data-ttu-id="d0d82-142">Кэширование фотографий пользователей</span><span class="sxs-lookup"><span data-stu-id="d0d82-142">Cache user photos</span></span>

<span data-ttu-id="d0d82-143">Exchange возвращает данные с типом контента Image/JPEG, а также коллекцию значений заголовков.</span><span class="sxs-lookup"><span data-stu-id="d0d82-143">Exchange returns the data with a content type of image/jpeg, along with a collection of header values.</span></span> <span data-ttu-id="d0d82-144">Заголовок **ETag** похож на ключ изменения.</span><span class="sxs-lookup"><span data-stu-id="d0d82-144">The **ETag** header is similar to a change key.</span></span> <span data-ttu-id="d0d82-145">Значение — это строка, представляющая время последнего обновления фотографии.</span><span class="sxs-lookup"><span data-stu-id="d0d82-145">The value is a string that represents the last time the photo was updated.</span></span> <span data-ttu-id="d0d82-146">**Тег eTag** остается таким же для фотографии пользователя, пока не будет изменена фотография.</span><span class="sxs-lookup"><span data-stu-id="d0d82-146">The **ETag** remains the same for the user photo until the photo is changed.</span></span> <span data-ttu-id="d0d82-147">Это значение **ETag** можно отправить на сервер в запросе HTTPS **Get** в заголовке **If – None – ПОИСКПОЗ** .</span><span class="sxs-lookup"><span data-stu-id="d0d82-147">You can send this **ETag** value to the server in the HTTPS **GET** request in an **If-None-Match** header.</span></span> <span data-ttu-id="d0d82-148">Если с момента последнего запроса фотография не изменилась, сервер ответит ответ HTTP 304, который показывает, что это так.</span><span class="sxs-lookup"><span data-stu-id="d0d82-148">If the photo hasn't changed since the last request, the server will respond with an HTTP 304 response that indicates as such.</span></span> <span data-ttu-id="d0d82-149">Это означает, что вы можете использовать фотографию пользователя, которую вы запросили и сохранили, вместо обработки новой.</span><span class="sxs-lookup"><span data-stu-id="d0d82-149">This means that you can use the user photo that you previously requested and saved rather than processing a new one.</span></span> 

<span data-ttu-id="d0d82-150"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="d0d82-150"><a name="bk_EWSMA"> </a></span></span>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a><span data-ttu-id="d0d82-151">Получение фотографии пользователя контакта с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="d0d82-151">Get a contact user photo by using EWS Managed API</span></span>

<span data-ttu-id="d0d82-152">Приложение может использовать управляемый API EWS для получения фотографий для контактов, если контакт хранится в папке контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0d82-152">Your application can use the EWS Managed API to retrieve photos for contacts, if the contact is stored in a contact folder in the user's mailbox.</span></span> <span data-ttu-id="d0d82-153">Для этого сначала найдите идентификатор **элемента для контакта, который необходимо** использовать.</span><span class="sxs-lookup"><span data-stu-id="d0d82-153">To do this, first, find the **ItemId** for the contact you want use.</span></span> <span data-ttu-id="d0d82-154">Затем после привязывания к этому контакту загрузите его в коллекцию вложений.</span><span class="sxs-lookup"><span data-stu-id="d0d82-154">Then, after you bind to that contact, load it to the attachments collection.</span></span> <span data-ttu-id="d0d82-155">Если у контакта есть фотография, фотография будет одним из вложений.</span><span class="sxs-lookup"><span data-stu-id="d0d82-155">If the contact has a photo, the photo will be one of the attachments.</span></span> <span data-ttu-id="d0d82-156">Пройдите по коллекции вложений, проверив значение свойства **исконтактфото** .</span><span class="sxs-lookup"><span data-stu-id="d0d82-156">Loop through the attachments collection, checking the value of the **IsContactPhoto** property.</span></span> <span data-ttu-id="d0d82-157">Когда вы найдете фотографию контакта, вы можете сохранить ее на локальном компьютере, и приложение сможет получить к нему доступ.</span><span class="sxs-lookup"><span data-stu-id="d0d82-157">When you find the contact photo, you can save it to your local computer, and your application can access it.</span></span> 
  
<span data-ttu-id="d0d82-158">Этот процесс показан в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="d0d82-158">The following example shows this process.</span></span> <span data-ttu-id="d0d82-159">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="d0d82-159">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<span data-ttu-id="d0d82-160"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="d0d82-160"><a name="bk_EWS"> </a></span></span>

## <a name="get-a-user-photo-by-using-ews"></a><span data-ttu-id="d0d82-161">Получение фотографии пользователя с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="d0d82-161">Get a user photo by using EWS</span></span>

<span data-ttu-id="d0d82-162">Если вы получаете фотографию пользователя из доменных служб Active Directory, вы можете использовать операцию [GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (если вы знаете адрес электронной почты) или операцию [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (если вы не знаете адрес электронной почты).</span><span class="sxs-lookup"><span data-stu-id="d0d82-162">If you're getting a user photo from AD DS, you can use the [GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) operation (if you know the email address) or the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation (if you don't know the email address).</span></span> <span data-ttu-id="d0d82-163">Если вы получаете фотографию пользователя из папки "Контакты" в почтовом ящике, используйте операцию [GetItem](https://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) , а затем операцию [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d0d82-163">If you're getting a user photo from a contacts folder in the mailbox, use the [GetItem](https://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) operation followed by the [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="d0d82-164">В обоих случаях фотография возвращается в виде строки в виде строки с кодировкой base64 в ответе XML.</span><span class="sxs-lookup"><span data-stu-id="d0d82-164">In either case, the photo is returned as a Base64-encoded string in the XML response.</span></span> 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a><span data-ttu-id="d0d82-165">Получение фотографии пользователя почтового ящика с помощью операции GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="d0d82-165">Get a mailbox user photo by using the GetUserPhoto operation</span></span>

<span data-ttu-id="d0d82-166">Использование операции **GetUserPhoto** является простым.</span><span class="sxs-lookup"><span data-stu-id="d0d82-166">Using the **GetUserPhoto** operation is straightforward.</span></span> <span data-ttu-id="d0d82-167">В XML-запросе укажите адрес электронной почты пользователя и размер возвращаемой [фотографии](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) (в элементе [сизерекуестед](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="d0d82-167">In the XML request, specify the email address of the user, and the [size of the photo](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) to return (in the [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element).</span></span> <span data-ttu-id="d0d82-168">В приведенном ниже примере XML-запроса показано, как получить фотографию для Ольга Даниелс шириной 360 пикселя на 360 пикселя высотой.</span><span class="sxs-lookup"><span data-stu-id="d0d82-168">The following XML request example shows how to get a photo for Sadie Daniels that's 360 pixels wide by 360 pixels high.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="d0d82-169">Ниже приведен XML-ответ.</span><span class="sxs-lookup"><span data-stu-id="d0d82-169">The following is the XML response.</span></span> <span data-ttu-id="d0d82-170">Фотография в кодировке Base64 хранится в элементе [PictureData](https://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (содержимое было сокращено для удобочитаемости).</span><span class="sxs-lookup"><span data-stu-id="d0d82-170">The Base64-encoded photo is contained in the [PictureData](https://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) element (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a><span data-ttu-id="d0d82-171">Получение фотографии пользователя почтового ящика с помощью операции ResolveNames</span><span class="sxs-lookup"><span data-stu-id="d0d82-171">Get a mailbox user photo by using the ResolveNames operation</span></span>

<span data-ttu-id="d0d82-172">Если вы не знаете адрес электронной почты пользователя, для которого вы получаете фотографию, вы можете [использовать операцию ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) , чтобы получить кандидатов для возможных сопоставлений.</span><span class="sxs-lookup"><span data-stu-id="d0d82-172">If you don't know the email address of the user for whom you are getting a photo, you can [use the ResolveNames operation](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) to get candidates for a possible match.</span></span> <span data-ttu-id="d0d82-173">Если для атрибута **контактдаташапе** элемента [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) задано значение "аллпропертиес", для каждого кандидата будет возвращено множество данных, включая фотографии пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0d82-173">If you specify "AllProperties" for the **ContactDataShape** attribute of the [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) element, a lot of data, including user photos, will be returned for each candidate.</span></span> <span data-ttu-id="d0d82-174">В следующем примере показан XML-запрос для разрешения имени "Ольга" и возврата всех свойств для каждого кандидата.</span><span class="sxs-lookup"><span data-stu-id="d0d82-174">The following example shows the XML request to resolve the name "Sadie" and return all the properties for each candidate.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d0d82-175">В ответе будет возвращено множество данных.</span><span class="sxs-lookup"><span data-stu-id="d0d82-175">A lot of data will be returned in the response.</span></span> <span data-ttu-id="d0d82-176">В приведенном ниже примере показаны только те данные, которые относятся к фотографии пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0d82-176">The following example shows only the data that is relevant to the user photo.</span></span> <span data-ttu-id="d0d82-177">Элемент **Photo** содержит фотографию пользователя с кодировкой base64 (содержимое было сокращено для удобочитаемости).</span><span class="sxs-lookup"><span data-stu-id="d0d82-177">The **Photo** element contains the Base64-encoded user photo (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a><span data-ttu-id="d0d82-178">Получение фотографии пользователя контакта с помощью операции GetAttachment</span><span class="sxs-lookup"><span data-stu-id="d0d82-178">Get a contact user photo by using the GetAttachment operation</span></span>

<span data-ttu-id="d0d82-179">С помощью EWS вы можете получать фотографии из контактов, хранящихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d0d82-179">You can use EWS to get photos from contacts stored in your mailbox.</span></span> <span data-ttu-id="d0d82-180">Для начала используйте операцию **GetItem** , чтобы возвратить все свойства, чтобы можно было искать фотографии.</span><span class="sxs-lookup"><span data-stu-id="d0d82-180">First, you use the **GetItem** operation to return all properties so you can look for photos.</span></span> <span data-ttu-id="d0d82-181">В следующем примере показан XML-запрос для получения элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="d0d82-181">The following example shows an XML request to get a contact item.</span></span> <span data-ttu-id="d0d82-182">Идентификатор элемента был сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0d82-182">The item ID has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="d0d82-183">Найдите элемент [хаспиктуре](https://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) , чтобы убедиться, что контакт имеет связанную фотографию.</span><span class="sxs-lookup"><span data-stu-id="d0d82-183">Look for the [HasPicture](https://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) element to verify that the contact has an associated photo.</span></span> <span data-ttu-id="d0d82-184">Затем просмотрите коллекцию вложений, для которой для элемента [исконтактфото](https://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) задано значение true.</span><span class="sxs-lookup"><span data-stu-id="d0d82-184">Then look through the collection of attachments for one that has a value of true for the [IsContactPhoto](https://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="d0d82-185">В приведенном ниже примере ответа показаны только нужные данные.</span><span class="sxs-lookup"><span data-stu-id="d0d82-185">The following response example shows only the relevant data.</span></span> <span data-ttu-id="d0d82-186">Значения ИДЕНТИФИКАТОРов сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0d82-186">The ID values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

Затем используйте операцию **GetAttachment** с **AttachmentId** , чтобы запросить вложение, имеющее фотографию контакта. В следующем примере показан XML-запрос для получения вложения. <span data-ttu-id="d0d82-189">Идентификатор сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0d82-189">The ID is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показан XML-ответ со сведениями о запрошенном вложении. <span data-ttu-id="d0d82-191">Элемент [Content](https://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) содержит строку в кодировке Base64 для фотографии пользователя, что в этом примере сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0d82-191">The [Content](https://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) element contains the Base64-encoded string for the user photo, shortened in this example for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="d0d82-192"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="d0d82-192"><a name="bk_EWS"> </a></span></span>

## <a name="decode-a-base64-encoded-string"></a><span data-ttu-id="d0d82-193">Декодирование строки в кодировке Base64</span><span class="sxs-lookup"><span data-stu-id="d0d82-193">Decode a Base64-encoded string</span></span>

<span data-ttu-id="d0d82-194">Независимо от того, какую операцию вы используете для получения фотографии пользователя, вам потребуется декодировать эту строку, чтобы ее можно было использовать в приложении.</span><span class="sxs-lookup"><span data-stu-id="d0d82-194">Regardless of the operation you use to get a user photo, you'll need to decode that string so you can use it in your application.</span></span> <span data-ttu-id="d0d82-195">В приведенном ниже примере показано, как декодировать строку, а затем сохранить ее на локальном компьютере, чтобы приложение могло получить к нему доступ позже.</span><span class="sxs-lookup"><span data-stu-id="d0d82-195">The following example shows how to decode the string, and then save it to your local computer so you application can access it later.</span></span>
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a><span data-ttu-id="d0d82-196">См. также</span><span class="sxs-lookup"><span data-stu-id="d0d82-196">See also</span></span>

- [<span data-ttu-id="d0d82-197">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="d0d82-197">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)    
- [<span data-ttu-id="d0d82-198">Устранение неоднозначности имен с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d0d82-198">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [<span data-ttu-id="d0d82-199">Пакетная обработка контактов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d0d82-199">Process contacts in batches by using EWS in Exchange</span></span>](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

