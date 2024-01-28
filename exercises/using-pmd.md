# Using PMD

Pick a Java project from Github (see the [instructions](../sujet.md) for suggestions). Run PMD on its source code using any ruleset. Describe below an issue found by PMD that you think should be solved (true positive) and include below the changes you would add to the source code. Describe below an issue found by PMD that is not worth solving (false positive). Explain why you would not solve this issue.

You can use the default [rule base](https://github.com/pmd/pmd/blob/master/pmd-java/src/main/resources/rulesets/java/quickstart.xml) available on the source repository of PMD.

## Answer

Command (see assets/pmd_cmd.txt) runned in javaparser-starter project using a complete ruleset found in the official git repo.
Output of the previous command can be found in the "assets/output" file.

An issue found that could be solved (true positive) would be :

LocalVariableCouldBeFinal:	Local variable 'file' could be declared final

This concerns a variable which could be declared final because the value stays the same during all the execution of our code, we just have to add final keyword.

An issue found that shloud not be solved (false positive) would be :

ShortClassName:	Avoid short class names like Main

I would not solve this issue because short class name are not necessarily bad, in this case : Main is comprehensive enough
because it concerns the main class executing all the code.