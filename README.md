# learnautomationdotnet
this project's purpose is to learn to write automation playwright with dot net C#

# Account

Username: automationdotnet

Password: HacLong@231

# Course

learning source: https://www.youtube.com/watch?v=5i53YLWD_QI&list=PL6tu16kXT9PoUv6HwexX5LPBzzv7QkI9W

# System requirements
Playwright is distributed as a .NET Standard 2.0 library. We recommend .NET 8.
Windows 10+, Windows Server 2016+ or Windows Subsystem for Linux (WSL).
MacOS 12 Monterey, MacOS 13 Ventura, or MacOS 14 Sonoma.
Debian 11, Debian 12, Ubuntu 20.04 or Ubuntu 22.04.

# tip
Can ask https://chatgpt.com/ when facing an error

# Require

1. Install playwright dot net in https://playwright.dev/dotnet/docs/intro website
2. Install Visual Studio 2019 or more (if cracked is better)
3. Install dotnet https://dotnet.microsoft.com/fr-fr/download/dotnet/thank-you/sdk-8.0.300-windows-x64-installer
4. Install PowerShell https://learn.microsoft.com/vi-vn/powershell/scripting/install/installing-powershell?view=powershell-7.4

# Command line:
dotnet test -- Run all tests
HEADED=1 dotnet test  -- Run your tests in headed mode (default headless mode)
BROWSER=webkit dotnet test  --  Run tests on different browsers: Browser env
dotnet test -- Playwright.BrowserName=webkit  --  Run tests on different browsers: launch configuration

# Run specific tests
1. To run a single test file, use the filter flag followed by the class name of the test you want to run.
dotnet test --filter "ExampleTest"
2. To run a set of test files, use the filter flag followed by the class names of the tests you want to run.
dotnet test --filter "ExampleTest1|ExampleTest2"
3. To run a test with a specific title use the filter flag followed by Name~ and the title of the test.
dotnet test --filter "Name~GetStartedLink"
4. Run tests with multiple workers
dotnet test -- NUnit.NumberOfTestWorkers=5
5. Debugging Tests
PWDEBUG=1 dotnet test
