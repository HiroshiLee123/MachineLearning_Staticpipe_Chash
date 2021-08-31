# MachineLearning_Staticpipe_Chash
# Link for the issue : https://github.com/dotnet/machinelearning/contribute
# In this Link the issue is to Right now  : we use TlcEnvironment (or ConsoleEnvironment) which outputs everything to console.
# And XUnit don't care about console, and if you want to look on output during test execution you need to do something like this:
# machinelearning/test/Microsoft.ML.StaticPipelineTesting/StaticPipeTests.cs
#
# Line 31 in 4cb7dd9
#
# Console.SetOut(_textWriter); 
# We should have XUnitEnvironment or TestEnvironment and redirect all output to ITestOutputHelper.
#------------------------------------------------------------------------------------------------------------------------------------------------------------
#------------------------------------------------------------------------------------------------------------------------------------------------------------
