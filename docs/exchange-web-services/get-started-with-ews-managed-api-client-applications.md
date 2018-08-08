---
title: Начало работы с клиентскими приложениями, использующими управляемый API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: Разработка простого почтового клиентского приложения Hello World для Exchange с помощью управляемого API EWS.
ms.openlocfilehash: b4254ab80b4dfc2c8fadf90c79d57517c3a0bb16
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353989"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a><span data-ttu-id="3c538-103">Начало работы с клиентскими приложениями, использующими управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="3c538-103">Get started with EWS Managed API client applications</span></span>

<span data-ttu-id="3c538-104">Разработка простого почтового клиентского приложения Hello World для Exchange с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-104">Develop a simple Hello World email client application for Exchange by using the EWS Managed API.</span></span> 
  
<span data-ttu-id="3c538-p101">[Управляемый API EWS](http://aka.ms/ews-managed-api-readme) предоставляет интуитивно понятную и простую в использовании объектную модель для отправки и получения сообщений веб-служб от клиентских приложений, приложений порталов и приложений-служб. Управляемый API EWS предоставляет вам доступ почти ко всем сведениям, хранящимся в Exchange Online, Exchange Online в составе Office 365 или почтовом ящике сервера Exchange. Вы можете использовать сведения из этой статьи при разработке своего первого клиентского приложения, использующего управляемый API EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-p101">The [EWS Managed API](http://aka.ms/ews-managed-api-readme) provides an intuitive, easy-to-use object model for sending and receiving web service messages from client applications, portal applications, and service applications. You can access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or an Exchange server mailbox by using the EWS Managed API. You can use the information in this article to help you develop your first EWS Managed API client application.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3c538-108">Управляемое API EWS теперь доступно в качестве проекта с открытым кодом на [GitHub](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="3c538-108">The EWS Managed API is now available as an open source project on  GitHub http://aka.ms/ews-managed-api-github . You can use the open source library to:</span></span> <span data-ttu-id="3c538-109">Вы можете использовать библиотеку открытого кода, чтобы:</span><span class="sxs-lookup"><span data-stu-id="3c538-109">You can use the open source library to:</span></span> 
> - <span data-ttu-id="3c538-110">добавлять исправления ошибок и улучшения в API;</span><span class="sxs-lookup"><span data-stu-id="3c538-110">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="3c538-111">получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске;</span><span class="sxs-lookup"><span data-stu-id="3c538-111">Get fixes and enhancements before they are available in an official release.</span></span> 
> - <span data-ttu-id="3c538-112">получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах.</span><span class="sxs-lookup"><span data-stu-id="3c538-112">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span> 
>
>  <span data-ttu-id="3c538-113">Мы будем рады вашему [вкладу](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="3c538-113">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="3c538-114">Вам потребуется сервер Exchange Server</span><span class="sxs-lookup"><span data-stu-id="3c538-114">You'll need an Exchange server</span></span>
<span data-ttu-id="3c538-115"><a name="NeedExchange"> </a></span><span class="sxs-lookup"><span data-stu-id="3c538-115"></span></span>

<span data-ttu-id="3c538-p103">Если у вас уже есть учетная запись почтового ящика Exchange, вы можете пропустить этот раздел. В противном случае у вас есть следующие варианты настройки почтового ящика Exchange для вашего первого клиентского приложения EWS:</span><span class="sxs-lookup"><span data-stu-id="3c538-p103">If you already have an Exchange mailbox account, you can skip this section. Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS client application:</span></span>
  
- <span data-ttu-id="3c538-p104">Заведите [сайт разработчиков Office 365](http://msdn.microsoft.com/ru-RU/library/office/fp179924.aspx) (рекомендуется). Это самый быстрый способ настройки почтового ящика Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c538-p104">Get an [Office 365 Developer Site](http://msdn.microsoft.com/ru-RU/library/office/fp179924.aspx) (recommended). This is the quickest way for you to set up an Exchange mailbox.</span></span> 
    
- <span data-ttu-id="3c538-120">Скачайте [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="3c538-120">Download [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>
    
<span data-ttu-id="3c538-p105">Убедившись, что вы можете отправлять и получать сообщения из Exchange, вы будете готовы настроить среду разработки. Вы можете использовать веб-клиент Exchange [Outlook Web App](http://technet.microsoft.com/ru-RU/library/jj657718%28v=exchg.150%29.aspx), чтобы убедиться, что вы можете отправлять сообщения.</span><span class="sxs-lookup"><span data-stu-id="3c538-p105">After you have verified that you can send and receive email from Exchange, you are ready to set up your development environment. You can use the Exchange web client [Outlook Web App](http://technet.microsoft.com/ru-RU/library/jj657718%28v=exchg.150%29.aspx) to verify that you can send email.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="3c538-123">Настройка среды разработки</span><span class="sxs-lookup"><span data-stu-id="3c538-123">Set up your development environment</span></span>
<span data-ttu-id="3c538-124"><a name="Setup"> </a></span><span class="sxs-lookup"><span data-stu-id="3c538-124"></span></span>

<span data-ttu-id="3c538-125">Убедитесь, что у вас есть доступ к следующим ресурсам:</span><span class="sxs-lookup"><span data-stu-id="3c538-125">Make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="3c538-p106">Любая версия [Visual Studio](http://www.visualstudio.com/ru-RU/downloads/download-visual-studio-vs.aspx), поддерживающая .NET Framework 4. Хотя на самом деле вам не требуется Visual Studio, ведь вы можете использовать любой компилятор C#, мы рекомендуем использовать его.</span><span class="sxs-lookup"><span data-stu-id="3c538-p106">Any version of [Visual Studio](http://www.visualstudio.com/ru-RU/downloads/download-visual-studio-vs.aspx) that supports the .NET Framework 4. Although technically, you don't need Visual Studio because you can use any C# compiler, we recommend that you use it.</span></span> 
    
- <span data-ttu-id="3c538-p107">[Управляемый API EWS](http://aka.ms/ews-managed-api-readme). Вы можете использовать 64- или 32-разрядную версию в зависимости от вашей системы. Используйте для установки папку по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c538-p107">The [EWS Managed API](http://aka.ms/ews-managed-api-readme). You can use either the 64-bit or 32-bit version, depending on your system. Use the default installation location.</span></span> 
    
## <a name="create-your-first-ews-managed-api-application"></a><span data-ttu-id="3c538-131">Создание первого приложения, использующего управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="3c538-131">Create your first EWS Managed API application</span></span>
<span data-ttu-id="3c538-132"><a name="Create"> </a></span><span class="sxs-lookup"><span data-stu-id="3c538-132"></span></span>

<span data-ttu-id="3c538-p108">В этом руководстве предполагается, что у вас настроен сайт разработчиков Office 365. Если вы скачали и установили Exchange, потребуется [установить действительный сертификат](http://technet.microsoft.com/ru-RU/library/bb310769%28v=exchg.141%29.aspx) на сервере Exchange или [реализовать обратный вызов проверки сертификатов](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) для самозаверяющего сертификата, предоставляемого по умолчанию. Обратите внимание, что эти действия могут слегка отличаться в зависимости от используемой версии Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="3c538-p108">These steps assume that you set up an Office 365 Developer Site. If you downloaded and installed Exchange, you will need to [install a valid certificate](http://technet.microsoft.com/ru-RU/library/bb310769%28v=exchg.141%29.aspx) on your Exchange server or [implement a certificate validation](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) callback for a self-signed certificate that is provided by default. Also note that these steps might vary slightly depending on the version of Visual Studio that you are using.</span></span> 
  
### <a name="step-1-create-a-project-in-visual-studio"></a><span data-ttu-id="3c538-136">Этап 1. Создание проекта в Visual Studio</span><span class="sxs-lookup"><span data-stu-id="3c538-136">Step 1: Create a project in Visual Studio</span></span>

1. <span data-ttu-id="3c538-p109">В Visual Studio выберите в меню **Файл** пункт **Создать**, а затем  **Проект**. Откроется диалоговое окно **Новый проект**.</span><span class="sxs-lookup"><span data-stu-id="3c538-p109">In Visual Studio, on the **File** menu, choose **New**, and then choose **Project**. The **New Project** dialog box opens.</span></span> 
    
2. <span data-ttu-id="3c538-p110">Создайте **Консольное приложение C#**. В панели **Шаблоны** выберите **Visual C#**, а затем  **Консольное приложение**.</span><span class="sxs-lookup"><span data-stu-id="3c538-p110">Create a **C# Console Application**. From the **Templates** pane, choose **Visual C#**, and then choose **Console Application**.</span></span> 
    
3. <span data-ttu-id="3c538-141">Назовите проект HelloWorld, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="3c538-141">Name the project HelloWorld, and then choose **OK**.</span></span>
    
<span data-ttu-id="3c538-142">Visual Studio создаст проект и откроет окно документа с кодом Program.cs.</span><span class="sxs-lookup"><span data-stu-id="3c538-142">Visual Studio creates the project and opens the Program.cs code document window.</span></span>

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a><span data-ttu-id="3c538-143">Этап 2. Добавление ссылки на управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="3c538-143">Step 2: Add a reference to the EWS Managed API</span></span>

1. <span data-ttu-id="3c538-p111">Если окно **обозревателя решений** уже открыто, пропустите этот этап и переходите к этапу 2. Чтобы открыть **обозреватель решений**, в меню **Вид** выберите пункт **Обозреватель решений**.</span><span class="sxs-lookup"><span data-stu-id="3c538-p111">If the **Solution Explorer** window is already open, skip this step and proceed to step 2. To open the **Solution Explorer** window, on the **View** menu, choose **Solution Explorer**.</span></span> 
    
2. <span data-ttu-id="3c538-p112">В **обозревателе решений** выберите проект **HelloWorld**, откройте контекстное меню (правая кнопка мыши) раздела **Ссылки** и выберите команду **Добавить ссылку**. Откроется диалоговое окно управления ссылками проекта.</span><span class="sxs-lookup"><span data-stu-id="3c538-p112">In the **Solution Explorer** and the **HelloWorld** project, open the shortcut menu (right-click) for **References** and choose **Add Reference** from the context menu. A dialog box for managing project references will open.</span></span> 
    
3. <span data-ttu-id="3c538-p113">Выберите команду **Обзор**. Перейдите в папку, где установлена DLL-библиотека управляемого API EWS. По умолчанию программа установки выбирает следующий путь: C:\Program Files\Microsoft\Exchange\Web Services\<версия>\. Путь может зависеть от того, скачали вы 32- или 64-разрядную версию файла Microsoft.Exchange.WebServices.dll. Выберите **Microsoft.Exchange.WebServices.dll** и нажмите кнопку **ОК** или **Добавить**. В проект будет добавлена ссылка на управляемый API EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-p113">Choose the **Browse** option. Browse to the location where you installed the EWS Managed API DLL. The default path set by the installer is the following: C:\Program Files\Microsoft\Exchange\Web Services\<version>\. The path can vary based on whether you download the 32 or 64 bit version of the Microsoft.Exchange.WebServices.dll. Choose **Microsoft.Exchange.WebServices.dll** and select **OK** or **Add**. This adds the EWS Managed API reference to your project.</span></span> 
    
4. <span data-ttu-id="3c538-p114">Если вы используете Управляемый API EWS 2.0, измените проект HelloWorld, чтобы он ссылался на .NET Framework 4. Другие версии управляемого API EWS могут использовать другую целевую версию .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="3c538-p114">If you are using EWS Managed API 2.0, change the HelloWorld project to target the .NET Framework 4. Other versions of the EWS Managed API might use a different target version of the .NET Framework.</span></span>
    
5. <span data-ttu-id="3c538-p115">Убедитесь, что вы используете правильную целевую версию .NET Framework. Откройте контекстное меню (правая кнопка мыши) проекта **HelloWorld** в **обозревателе решений** и выберите пункт **Свойства**. Убедитесь, что в раскрывающемся списке **Целевая рабочая среда** выбран пункт **.NET Framework 4**.</span><span class="sxs-lookup"><span data-stu-id="3c538-p115">Confirm that you are using the correct target version of the .NET Framework. Open the shortcut menu (right-click) for your **HelloWorld** project in the **Solution Explorer**, and choose **Properties**. Verify that the **.NET Framework 4** is selected in the **Target framework** drop-down box.</span></span> 
    
<span data-ttu-id="3c538-159">Теперь, когда у вас есть настройка проекта и вы создали ссылку на управляемое API EWS, то вы готовы создать свое первое приложение.</span><span class="sxs-lookup"><span data-stu-id="3c538-159">Now that you have your project set up and you created a reference to the EWS Managed API, you are ready to create your first application.</span></span> <span data-ttu-id="3c538-160">Для простоты работы добавьте код в файл Program.cs.</span><span class="sxs-lookup"><span data-stu-id="3c538-160">To keep things simple, add your code to the Program.cs file.</span></span> <span data-ttu-id="3c538-161">Ознакомьтесь со статьей [Ссылка на сборку управляемого API EWS](how-to-reference-the-ews-managed-api-assembly.md) для получения дополнительной информации о ссылках на управляемое API EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-161">Read [Reference the EWS Managed API assembly](how-to-reference-the-ews-managed-api-assembly.md) for more information about referencing the EWS Managed API.</span></span> <span data-ttu-id="3c538-162">На следующем этапе вы будете разрабатывать базовый код, чтобы создавать большинство клиентских приложений управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-162">In the next step, you will develop the basic code to write most EWS Managed API client applications.</span></span> 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a><span data-ttu-id="3c538-163">Этап 3. Настройка проверки перенаправления URL-адресов для автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3c538-163">Step 3: Set up URL redirection validation for Autodiscover</span></span>

- <span data-ttu-id="3c538-p117">Добавьте приведенный ниже метод обратного вызова для проверки перенаправления после метода **Main(string[] args)**. Он проверяет, представляют ли перенаправленные URL-адреса, возвращенные функцией [автообнаружения](autodiscover-for-exchange.md), конечную точку HTTPS.</span><span class="sxs-lookup"><span data-stu-id="3c538-p117">Add the following redirection validation callback method after the **Main(string[] args)** method. This validates whether redirected URLs returned by [Autodiscover](autodiscover-for-exchange.md) represent an HTTPS endpoint.</span></span> 
    
  ```cs
  private static bool RedirectionUrlValidationCallback(string redirectionUrl)
  {
     // The default for the validation callback is to reject the URL.
     bool result = false;
     Uri redirectionUri = new Uri(redirectionUrl);
     // Validate the contents of the redirection URL. In this simple validation
     // callback, the redirection URL is considered valid if it is using HTTPS
     // to encrypt the authentication credentials. 
     if (redirectionUri.Scheme == "https")
     {
        result = true;
     }
     return result;
  }
  ```

<span data-ttu-id="3c538-p118">Этот проверяющий метод обратного вызова будет передан объекту **ExchangeService** на этапе 4. Это необходимо, чтобы ваше приложение доверяло и следовало перенаправлению функции автообнаружения  результат перенаправления функции автообнаружения предоставляет конечную точку EWS для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="3c538-p118">This validation callback will be passed to the **ExchangeService** object in step 4. You need this so that your application will trust and follow Autodiscover redirects - the results of the Autodiscover redirect provides the EWS endpoint for our application.</span></span> 

### <a name="step-4-prepare-the-exchangeservice-object"></a><span data-ttu-id="3c538-168">Этап 4. Подготовка объекта ExchangeService</span><span class="sxs-lookup"><span data-stu-id="3c538-168">Step 4: Prepare the ExchangeService object</span></span>

1. <span data-ttu-id="3c538-p119">Добавьте ссылку на директиву **using** в управляемый API EWS. Добавьте следующий код после директивы **using** в начале файла Program.cs.</span><span class="sxs-lookup"><span data-stu-id="3c538-p119">Add a **using** directive reference to the EWS Managed API. Add the following code after the last **using** directive at the top of Program.cs.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. <span data-ttu-id="3c538-p120">В методе **Main** создайте экземпляр объекта [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в нужной версией службы. В этом примере используется самая ранняя версия схемы EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-p120">In the **Main** method, instantiate the [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object with the service version you intend to target. This example targets the earliest version of the EWS schema.</span></span> 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. <span data-ttu-id="3c538-p121">Если вы ссылаетесь на локальный сервер Exchange и ваш клиент присоединен к домену, переходите к этапу 4. Если ваш клиент ссылается на почтовый ящик Exchange Online или сайта разработчиков Office 365, необходимо передавать учетные данные в явной форме. Добавьте следующий код после создания экземпляра объекта **ExchangeService** и задайте данные учетной записи почтового ящика. Имя пользователя должно быть именем участника-пользователя. Переходите к этапу 5.</span><span class="sxs-lookup"><span data-stu-id="3c538-p121">If you are targeting an on-premises Exchange server and your client is domain joined, proceed to step 4. If you client is targeting an Exchange Online or Office 365 Developer Site mailbox, you have to pass explicit credentials. Add the following code after the instantiation of the **ExchangeService** object and set the credentials for your mailbox account. The user name should be the user principal name. Proceed to step 5.</span></span> 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. <span data-ttu-id="3c538-p122">Присоединенные к доменам клиенты, которые ссылаются на локальный сервер Exchange, могут использовать заданные по умолчанию учетные данные пользователя, выполнившего вход, при условии, что учетные данные связаны с почтовым ящиком. Добавьте следующий код после создания экземпляра объекта **ExchangeService**.</span><span class="sxs-lookup"><span data-stu-id="3c538-p122">Domain-joined clients that target an on-premises Exchange server can use the default credentials of the user who is logged on, assuming the credentials are associated with a mailbox. Add the following code after the instantiation of the **ExchangeService** object.</span></span> 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   <span data-ttu-id="3c538-p123">Если ваш клиент ссылается на почтовый ящик Exchange Online или сайта разработчиков Office 365, убедитесь, что для параметра [UseDefaultCredentials](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) задано значение **false**, установленное по умолчанию. Ваш клиент готов совершить первый вызов службы автообнаружения, чтобы получить URL-адрес службы для вызовов службы EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-p123">If your client targets an Exchange Online or Office 365 Developer Site mailbox, verify that [UseDefaultCredentials](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) is set to **false**, which is the default value. Your client is ready to make the first call to the Autodiscover service to get the service URL for calls to the EWS service.</span></span>
    
5. <span data-ttu-id="3c538-p124">Метод **AutodiscoverUrl** объекта **ExchangeService** совершает серию вызовов службы автообнаружения, чтобы получить URL-адрес службы. Если вызов этого метода совершен успешно, для свойства URL объекта **ExchangeService** будет задано значение URL-адреса службы. Передайте адрес электронной почты пользователя и **RedirectionUrlValidationCallback** методу **AutodiscoverUrl**. Добавьте приведенный ниже код после указания учетных данных на этапе 3 или 4. Измените  `user1@contoso.com` на ваш адрес электронной почты, чтобы служба автообнаружения нашла конечную точку EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-p124">The **AutodiscoverUrl** method on the **ExchangeService** object performs a series of calls to the Autodiscover service to get the service URL. If this method call is successful, the URL property on the **ExchangeService** object will be set with the service URL. Pass the user's email address and the **RedirectionUrlValidationCallback** to the **AutodiscoverUrl** method. Add the following code after the credentials have been specified in step 3 or 4. Change  `user1@contoso.com` to your email address so that the Autodiscover service finds your EWS endpoint.</span></span> 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

<span data-ttu-id="3c538-187">На этом этапе ваш клиент настроен для вызовов EWS для доступа к данным почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3c538-187">At this point, your client is set up to make calls to EWS to access mailbox data.</span></span> <span data-ttu-id="3c538-188">Если вы сейчас запустите свой код, то сможете проверить, что метод вызова **AutodiscoverUrl** отработал, проверив содержимое свойства [ExchangeService.Url](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3c538-188">If you run your code now, you can verify that the **AutodiscoverUrl** method call worked by examining the contents of the [ExchangeService.Url](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="3c538-189">Если это свойство содержит URL-адрес, то ваш вызов был удачным!</span><span class="sxs-lookup"><span data-stu-id="3c538-189">If this property contains a URL, your call was a success!</span></span> <span data-ttu-id="3c538-190">Это означает, что ваше приложение успешно прошло проверку подлинности службой и обнаружило конечную точку EWS для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3c538-190">This means that your application successfully authenticated with the service and discovered the EWS endpoint for your mailbox.</span></span> <span data-ttu-id="3c538-191">Теперь вы готовы выполнить первый вызов EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-191">Now you are ready to make your first calls to EWS.</span></span> <span data-ttu-id="3c538-192">Ознакомьтесь со статьей [Настройка URL-адреса службы EWS с помощью управляемого API EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) для получения дополнительной информации о настройке URL-адреса EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-192">Read [Set the EWS service URL by using the EWS Managed API](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) for more information about setting the EWS URL.</span></span> 

### <a name="step-6-create-your-first-hello-world-email-message"></a><span data-ttu-id="3c538-193">Этап 6. Создание первого сообщения электронной почты Hello World</span><span class="sxs-lookup"><span data-stu-id="3c538-193">Step 6: Create your first Hello World email message</span></span>

1. <span data-ttu-id="3c538-194">После вызова метода **AutodiscoverUrl** создайте новый экземпляр объекта **EmailMessage** и передайте созданный ранее объект службы.</span><span class="sxs-lookup"><span data-stu-id="3c538-194">After the **AutodiscoverUrl** method call, instantiate a new **EmailMessage** object and pass in the service object you created.</span></span> 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   <span data-ttu-id="3c538-p126">Теперь у вас есть сообщение электронной почты, в котором задана привязка к службе. Вызовы, совершенные из объекта **EmailMessage**, будут адресованы службе.</span><span class="sxs-lookup"><span data-stu-id="3c538-p126">You now have an email message on which the service binding is set. Any calls initiated on the **EmailMessage** object will be targeted at the service.</span></span> 
    
2. <span data-ttu-id="3c538-p127">Теперь задайте получателя сообщения. Для этого замените  `user1@contoso.com` на ваш SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="3c538-p127">Now set the To: line recipient of the email message. To do this, change  `user1@contoso.com` to use your SMTP address.</span></span> 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. <span data-ttu-id="3c538-199">Задайте тему и основной текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="3c538-199">Set the subject and the body of the email message.</span></span>
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. <span data-ttu-id="3c538-200">Теперь вы готовы отправить первое сообщение электронной почты с помощью службы управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="3c538-200">You are now ready to send your first email message by using the EWS Managed API.</span></span> <span data-ttu-id="3c538-201">Метод **Send** вызовет службу и отправит сообщение электронной почты для доставки.</span><span class="sxs-lookup"><span data-stu-id="3c538-201">The **Send** method will call the service and submit the email message for delivery.</span></span> <span data-ttu-id="3c538-202">Ознакомьтесь со статьей [Взаимодействие с EWS с помощью управляемого API EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) для получения дополнительной информации о других методах, которые можно использовать для взаимодействия с Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c538-202">Read [Communicate with EWS by using the EWS Managed API](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) to learn about other methods you can use to communicate with Exchange.</span></span> 
    
   ```cs
    email.Send();
   ```

5. <span data-ttu-id="3c538-p129">Вы готовы запустить свое приложение Hello World. В Visual Studio нажмите клавишу **F5**. Откроется пустое окно консоли. В окно консоли не будет появляться никакого текста, пока приложение проходит проверку подлинности, следует перенаправлению службы автообнаружения, а затем совершает первый вызов для создания сообщения электронной почты, которое вы отправляете себе. Если вы хотите увидеть совершаемые вызовы, добавьте две приведенные ниже строки кода перед вызовом метода **AutodiscoverUrl**. Затем нажмите клавишу F5. [Запросы и ответы EWS будут трассированы](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) в окне консоли.</span><span class="sxs-lookup"><span data-stu-id="3c538-p129">You are ready to run your Hello World application. In Visual Studio, select **F5**. A blank console window will open. You will not see anything in the console window while your application authenticates, follows Autodiscover redirections, and then makes its first call to create an email message that you send to yourself. If you want to see the calls being made, add the following two lines of code before the **AutodiscoverUrl** method is called. Then press F5. This will [trace out the EWS requests and responses](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) to the console window.</span></span> 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

<span data-ttu-id="3c538-p130">Теперь у вас есть работоспособное приложение, использующее управляемый API EWS. Для вашего удобства в следующем примере показан весь код, добавленный в файл Program.cs для создания приложения Hello World.</span><span class="sxs-lookup"><span data-stu-id="3c538-p130">You now have a working EWS Managed API client application. For your convenience, the following example shows all the code that you added to Program.cs to create your Hello World application.</span></span>

```cs
using System;
using Microsoft.Exchange.WebServices.Data;
namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
      service.Credentials = new WebCredentials("user1@contoso.com", "password");
      service.TraceEnabled = true;
      service.TraceFlags = TraceFlags.All;
      service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
      EmailMessage email = new EmailMessage(service);
      email.ToRecipients.Add("user1@contoso.com");
      email.Subject = "HelloWorld";
      email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API");
      email.Send();
    }
    private static bool RedirectionUrlValidationCallback(string redirectionUrl)
    {
      // The default for the validation callback is to reject the URL.
      bool result = false;
      Uri redirectionUri = new Uri(redirectionUrl);
      // Validate the contents of the redirection URL. In this simple validation
      // callback, the redirection URL is considered valid if it is using HTTPS
      // to encrypt the authentication credentials. 
      if (redirectionUri.Scheme == "https")
      {
        result = true;
      }
      return result;
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="3c538-212">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3c538-212">Next steps</span></span>
<span data-ttu-id="3c538-213"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="3c538-213"></span></span>

<span data-ttu-id="3c538-214">Если вы готовы усовершенствовать свое первое клиентское приложение с использованием управляемого API EWS, изучите следующие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="3c538-214">If you're ready to do more with your first EWS Managed API client application, explore the following resources:</span></span>
  
- [<span data-ttu-id="3c538-215">Exchange 2013: базовые примеры кода</span><span class="sxs-lookup"><span data-stu-id="3c538-215">Exchange 2013: 101 code samples</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)   
- [<span data-ttu-id="3c538-216">Папки и элементы</span><span class="sxs-lookup"><span data-stu-id="3c538-216">Folders and items</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="3c538-217">EWSEditor</span><span class="sxs-lookup"><span data-stu-id="3c538-217">EWSEditor</span></span>](http://ewseditor.codeplex.com/)
    
<span data-ttu-id="3c538-218">Если с приложением возникли проблемы, [попробуйте опубликовать вопрос или комментарий на форуме](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (и не забудьте прочитать первое сообщение).</span><span class="sxs-lookup"><span data-stu-id="3c538-218">If you run into any issues with your application, [try posting a question or comment in the forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (and don't forget to read the top post).</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="3c538-219">В этой статье</span><span class="sxs-lookup"><span data-stu-id="3c538-219">In this section</span></span>
<span data-ttu-id="3c538-220"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="3c538-220"></span></span>

- [<span data-ttu-id="3c538-221">Ссылка на сборку управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="3c538-221">How to: Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)   
- [<span data-ttu-id="3c538-222">Настройка URL-адреса службы EWS с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="3c538-222">How to: Set the EWS service URL by using the EWS Managed API</span></span>](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)   
- [<span data-ttu-id="3c538-223">Взаимодействие с EWS с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="3c538-223">How to: Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a><span data-ttu-id="3c538-224">См. также</span><span class="sxs-lookup"><span data-stu-id="3c538-224">See also</span></span>

- [<span data-ttu-id="3c538-225">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="3c538-225">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)    
- [<span data-ttu-id="3c538-226">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="3c538-226">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)    
- [<span data-ttu-id="3c538-227">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="3c538-227">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)   
- [<span data-ttu-id="3c538-228">Трассировка запросов и ответов для устранения неполадок в приложениях управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="3c538-228">How to: Trace requests and responses to troubleshoot EWS Managed API applications</span></span>](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

