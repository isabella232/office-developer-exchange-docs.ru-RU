---
title: Ссылки на сборку управляемого интерфейса API веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Найдите сведения о том, как ссылки на сборку управляемого интерфейса API веб-служб Exchange.
ms.openlocfilehash: a08ce43d139440186f611049fa1e457ea44f0362
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353688"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="95c89-103">Ссылки на сборку управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="95c89-103">Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="95c89-104">Найдите сведения о том, как ссылки на сборку управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="95c89-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="95c89-105">Управляемый API веб-служб Exchange предоставляет простой и полнофункциональных интерфейс для разработки и расширения приложений, использующих веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="95c89-105">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS).</span></span> <span data-ttu-id="95c89-106">С помощью Visual Studio или другой редактор кода, чтобы разрабатывать приложения управляемый API веб-служб Exchange, необходимо создать ссылку на сборку управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="95c89-106">Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly.</span></span> <span data-ttu-id="95c89-107">Если вы еще не установили уже управляемый API веб-служб Exchange, необходимо [загрузить API-интерфейса](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="95c89-107">If you haven't installed the EWS Managed API already, be sure to [download the API](http://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
> <span data-ttu-id="95c89-108">Управляемый API EWS теперь доступен в качестве проекта с открытым кодом на [репозиториев](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="95c89-108">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api).</span></span> <span data-ttu-id="95c89-109">Можно использовать библиотеку открытым кодом на:</span><span class="sxs-lookup"><span data-stu-id="95c89-109">You can use the open source library to:</span></span> 
> - <span data-ttu-id="95c89-110">добавлять исправления ошибок и улучшения в API;</span><span class="sxs-lookup"><span data-stu-id="95c89-110">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="95c89-111">получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске;</span><span class="sxs-lookup"><span data-stu-id="95c89-111">Get fixes and enhancements before they are available in an official release.</span></span> 
> - <span data-ttu-id="95c89-112">получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах.</span><span class="sxs-lookup"><span data-stu-id="95c89-112">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span>
> 
>  <span data-ttu-id="95c89-113">Мы будем рады [Ввод данных](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) с помощью репозиториев.</span><span class="sxs-lookup"><span data-stu-id="95c89-113">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="95c89-114">Создание ссылок на сборки</span><span class="sxs-lookup"><span data-stu-id="95c89-114">Referencing the assembly</span></span>

<span data-ttu-id="95c89-115">Чаще всего для добавления ссылки является использование Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="95c89-115">The most common way to add a reference is to use Visual Studio.</span></span> <span data-ttu-id="95c89-116">Мы знаем, что некоторые разработчиков предпочитают других редакторах, поэтому мы включая инструкции по использованию командной строки компилятора, а также инструкции по использованию Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="95c89-116">We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio.</span></span> <span data-ttu-id="95c89-117">Пользователь может заметить, что ниже примерах кода имеют те же **с помощью** инструкции.</span><span class="sxs-lookup"><span data-stu-id="95c89-117">You might notice that the code examples that follow have the same **using** statements.</span></span> <span data-ttu-id="95c89-118">Различие между двумя методами — это, что компилятор командной строки необходимо указать расположение файла сборки.</span><span class="sxs-lookup"><span data-stu-id="95c89-118">The difference between the two methods is that the command-line compiler needs the location of the assembly file.</span></span> <span data-ttu-id="95c89-119">Справочник по Visual Studio выполняет это автоматически в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="95c89-119">The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="95c89-120">Чтобы добавить ссылку с помощью Visual Studio</span><span class="sxs-lookup"><span data-stu-id="95c89-120">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="95c89-121">Скопируйте файл Microsoft.Exchange.WebServices.dll и файл Microsoft.Exchange.WebServices.xml в папку по выбору.</span><span class="sxs-lookup"><span data-stu-id="95c89-121">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice.</span></span> <span data-ttu-id="95c89-122">По умолчанию файлы устанавливаются в `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, но могут сохранять файлы в любом месте на вашем компьютере.</span><span class="sxs-lookup"><span data-stu-id="95c89-122">By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="95c89-123">В области обозреватель решений в Visual Studio выберите **ссылки**и затем выберите команду **Добавить ссылку**.</span><span class="sxs-lookup"><span data-stu-id="95c89-123">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**.</span></span> <span data-ttu-id="95c89-124">Откроется диалоговое окно Добавить ссылку.</span><span class="sxs-lookup"><span data-stu-id="95c89-124">This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="95c89-125">В окне Добавить ссылку, перейдите на вкладку **Обзор** , перейдите к местоположению файла Microsoft.Exchange.WebServices.dll, выберите этот файл и нажмите кнопку « **ОК»**.</span><span class="sxs-lookup"><span data-stu-id="95c89-125">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="95c89-126">Чтобы использовать управляемый API EWS в приложении, добавьте оператор **using** для пространства имен **Microsoft.Exchange.WebServices.Data** .</span><span class="sxs-lookup"><span data-stu-id="95c89-126">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="95c89-127">Чтобы добавить ссылку и выполните построение приложения с помощью командной строки компилятора</span><span class="sxs-lookup"><span data-stu-id="95c89-127">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="95c89-128">Поместите файл Microsoft.Exchange.WebServices.dll в папку по выбору.</span><span class="sxs-lookup"><span data-stu-id="95c89-128">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice.</span></span> <span data-ttu-id="95c89-129">Эта папка будет папку выходных данных для компилятора.</span><span class="sxs-lookup"><span data-stu-id="95c89-129">This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="95c89-130">В редакторе исходного кода добавьте оператор **using** в исходный код для пространства имен **Microsoft.Exchange.WebServices.Data** .</span><span class="sxs-lookup"><span data-stu-id="95c89-130">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="95c89-131">Запуск командной строки компилятора для построения приложения.</span><span class="sxs-lookup"><span data-stu-id="95c89-131">Run the command-line compiler to build the application.</span></span> <span data-ttu-id="95c89-132">В следующей команде используется компилятора .NET Framework C# для создания приложений Windows, определенных в файле исходного кода «program.cs».</span><span class="sxs-lookup"><span data-stu-id="95c89-132">The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs".</span></span> <span data-ttu-id="95c89-133">Предполагается, что компилятор расположен в каталоге установки по умолчанию и, что файл Microsoft.Exchange.WebServices.dll находится в подкаталоге текущий каталог с именем «создать».</span><span class="sxs-lookup"><span data-stu-id="95c89-133">It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="95c89-134">См. также</span><span class="sxs-lookup"><span data-stu-id="95c89-134">See also</span></span>

- [<span data-ttu-id="95c89-135">Начало работы с клиентскими приложениями, использующими управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="95c89-135">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="95c89-136">Настройка среды разработки приложений Exchange</span><span class="sxs-lookup"><span data-stu-id="95c89-136">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="95c89-137">Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="95c89-137">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

