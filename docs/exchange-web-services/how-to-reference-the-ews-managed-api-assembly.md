---
title: Ссылка на сборку управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Сведения о том, как ссылаться на сборку управляемого API EWS.
localization_priority: Priority
ms.openlocfilehash: d49091781da279d87a1eab35608f19ece43a0333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527763"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="be901-103">Ссылка на сборку управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="be901-103">Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="be901-104">Сведения о том, как ссылаться на сборку управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="be901-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="be901-105">Управляемый API EWS предоставляет простой и полнофункциональный интерфейс для разработки и расширения приложений, использующих веб-службы Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="be901-105">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS).</span></span> <span data-ttu-id="be901-106">Если вы используете Visual Studio или другой редактор кода для разработки приложения управляемого API EWS, вам потребуется создать ссылку на сборку управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="be901-106">Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly.</span></span> <span data-ttu-id="be901-107">Если вы еще не установили управляемый API EWS, обязательно [Скачайте API](https://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="be901-107">If you haven't installed the EWS Managed API already, be sure to [download the API](https://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
> <span data-ttu-id="be901-108">Управляемое API EWS теперь доступно в качестве проекта с открытым кодом на [GitHub](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="be901-108">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api).</span></span> <span data-ttu-id="be901-109">Вы можете использовать библиотеку открытого кода, чтобы:</span><span class="sxs-lookup"><span data-stu-id="be901-109">You can use the open source library to:</span></span> 
> - <span data-ttu-id="be901-110">добавлять исправления ошибок и улучшения в API;</span><span class="sxs-lookup"><span data-stu-id="be901-110">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="be901-111">получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске;</span><span class="sxs-lookup"><span data-stu-id="be901-111">Get fixes and enhancements before they are available in an official release.</span></span> 
> - <span data-ttu-id="be901-112">получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах.</span><span class="sxs-lookup"><span data-stu-id="be901-112">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span>
> 
>  <span data-ttu-id="be901-113">Мы будем рады вашему [вкладу](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) в GitHub.</span><span class="sxs-lookup"><span data-stu-id="be901-113">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="be901-114">Ссылка на сборку</span><span class="sxs-lookup"><span data-stu-id="be901-114">Referencing the assembly</span></span>

<span data-ttu-id="be901-115">Наиболее распространенный способ добавления ссылки — использование Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="be901-115">The most common way to add a reference is to use Visual Studio.</span></span> <span data-ttu-id="be901-116">Мы знаем, что некоторые разработчики хотели бы использовать другие редакторы, поэтому мы предоставляем инструкции по использованию компилятора командной строки, а также инструкции по использованию Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="be901-116">We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio.</span></span> <span data-ttu-id="be901-117">Вы можете заметить, что в приведенных ниже примерах кода **используются** одни и те же операторы using.</span><span class="sxs-lookup"><span data-stu-id="be901-117">You might notice that the code examples that follow have the same **using** statements.</span></span> <span data-ttu-id="be901-118">Разница между этими двумя методами состоит в том, что компилятору командной строки требуется расположение файла сборки.</span><span class="sxs-lookup"><span data-stu-id="be901-118">The difference between the two methods is that the command-line compiler needs the location of the assembly file.</span></span> <span data-ttu-id="be901-119">Справка по Visual Studio обрабатывает это в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="be901-119">The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="be901-120">Добавление ссылки с помощью Visual Studio</span><span class="sxs-lookup"><span data-stu-id="be901-120">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="be901-121">Поместите файл Microsoft. Exchange. WebServices. dll и Microsoft. Exchange. WebServices. XML в выбранную папку.</span><span class="sxs-lookup"><span data-stu-id="be901-121">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice.</span></span> <span data-ttu-id="be901-122">По умолчанию файлы установлены в `C:\Program Files\Microsoft\Exchange\Web Services\2.0\` , но их можно хранить в любом месте на компьютере.</span><span class="sxs-lookup"><span data-stu-id="be901-122">By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="be901-123">В области Обозреватель решений в Visual Studio выберите **ссылки**, а затем нажмите кнопку **Добавить ссылку**.</span><span class="sxs-lookup"><span data-stu-id="be901-123">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**.</span></span> <span data-ttu-id="be901-124">Откроется окно Добавить ссылку.</span><span class="sxs-lookup"><span data-stu-id="be901-124">This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="be901-125">В окне Добавить ссылку перейдите на вкладку **Обзор** , перейдите к расположению файла Microsoft. Exchange. WebServices. dll, выберите этот файл и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="be901-125">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="be901-126">Чтобы использовать управляемый API EWS в приложении, добавьте инструкцию **using** для пространства имен **Microsoft. Exchange. WebServices. Data** .</span><span class="sxs-lookup"><span data-stu-id="be901-126">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="be901-127">Добавление ссылки и построение приложения с помощью компилятора командной строки</span><span class="sxs-lookup"><span data-stu-id="be901-127">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="be901-128">Поместите файл Microsoft. Exchange. WebServices. dll в выбранную папку.</span><span class="sxs-lookup"><span data-stu-id="be901-128">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice.</span></span> <span data-ttu-id="be901-129">Эта папка будет выходной папкой для компилятора.</span><span class="sxs-lookup"><span data-stu-id="be901-129">This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="be901-130">В редакторе исходного кода добавьте оператор **using** в исходный код для пространства имен **Microsoft. Exchange. WebServices. Data** .</span><span class="sxs-lookup"><span data-stu-id="be901-130">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="be901-131">Запустите компилятор командной строки, чтобы создать приложение.</span><span class="sxs-lookup"><span data-stu-id="be901-131">Run the command-line compiler to build the application.</span></span> <span data-ttu-id="be901-132">Следующая команда использует компилятор C# .NET Framework для создания приложения Windows, определенного в файле исходного кода "program.cs".</span><span class="sxs-lookup"><span data-stu-id="be901-132">The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs".</span></span> <span data-ttu-id="be901-133">Предполагается, что компилятор находится в каталоге установки по умолчанию, а файл Microsoft. Exchange. WebServices. DLL находится в подкаталоге текущего каталога с именем "Build".</span><span class="sxs-lookup"><span data-stu-id="be901-133">It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="be901-134">См. также</span><span class="sxs-lookup"><span data-stu-id="be901-134">See also</span></span>

- [<span data-ttu-id="be901-135">Начало работы с клиентскими приложениями, использующими управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="be901-135">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="be901-136">Настройка среды разработки приложений Exchange</span><span class="sxs-lookup"><span data-stu-id="be901-136">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="be901-137">Взаимодействие с EWS с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="be901-137">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

