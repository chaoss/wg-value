## 1. Description
How much of a given code base is covered by at least one test suite. There are
two principle measures of test coverage. One is the percentage of
**subroutines** covered in a test suite run against a repository. The other
principle expression of test coverage is the percentage of **statements**
covered during the execution of a test suite. The CHAOSS metric definition for
"Test Coverage" includes both of these discrete measures. 

Programming languages refer to **subroutines** specifically as "functions",
"methods", "routines" or, in some cases, "subprograms." The percentage of
coverage for a particular repository is constrained in this definition to
methods defined within a specific repository, and does not include coverage of
libraries or other software upon which the repository is dependent. 

**Statements** include variable assignments, loop declarations, calls to system
functions, "go to" statements, and the common `return` statement at the
completion of a function or method, which may or may not include the return of
a `value` or `array of values`. 

## 2. Use Cases
An open source software package is being considered for deployment in a health
care provider's production ecosystem. As part of the product evaluation
process, IT Managers are comparing the test coverage of several alternate
systems. 

## 3. Formula

### Subroutine Coverage

![](./images/subroutine-coverage.png)

### Statement Coverage 

![](./images/statement-coverage.png)

## 4. Sample Filter and Visualization

### Filters
1. Time: Changes in test coverage over time provide evidence of project attention to maximizing overall test coverage. Specific parameters include `start date` and `end date` for the time period. 
2. Code_File: Each repository contains a number of files containing code. Filtering coverage by specific file provides a more granular view of test coverage. Some functions or statements may lead to more severe software failures than others. For example, untested code in the `fail safe` functions of a safety critical system are more important to test than `font color` function testing. 
3. Programming_Language: Most contemporary open source software repositories contain several different programming languages. The coverage percentage of each `Code_File` 

### Visualization 
1. Standard line graphs when time is included as a filter
2. Standard histograms or stacked bar charts for point in time coverage comparisons

## 5. Sample Implementation
Metrics tools will need to provide abstracted frameworks for representing test coverage because the tools used for measuring both `statement test coverage` and `subroutine test coverage` are programming language specific. 

## 6. Known Implementations
1. Augur has test coverage implemented as a table that is a child of the main repository table in its repository.  The data structure is illustrated below. Note that each time test coverage is tested, a record is made for each file tested, the testing tool used for testing and the number of statements/subroutines in the file, as well as the number of statements and subroutines tested. By recording test data at this level of granularity, Augur enables `Code_File` and `Programming_Language` summary level statistics and filters. 

![](./images/test_coverage_data_model.png)


## 7. Test Cases (Examples)
Test coverage examples are all programming language specific.  We provide a few examples here: 
1. [Python's primary testing framework is PyTest](https://docs.pytest.org/en/latest/)
2. [The Flask web framework for python enables coverage testing](http://flask.pocoo.org/docs/1.0/tutorial/tests/)
3. [Open source code coverage tools for common languages like Java, C, and C++ are available from my sites, including this one.](https://stackify.com/code-coverage-tools/#OpenSource)

## 8. External References (Literature)
Discussion of testing coverage as a measure of software quality and reliability is extensive and ongoing in the software engineering research literature. Some of the more canonical papers are listed below. 

1. J.H. Andrews, L.C. Briand, Y. Labiche, and A.S. Namin. 2006. Using Mutation Analysis for Assessing and Comparing Testing Coverage Criteria. IEEE Transactions on Software Engineering 32, 8: 608–624. https://doi.org/10.1109/TSE.2006.83
2. Phyllis G Frankl and Oleg Iakounenko. 1998. Further Empirical Studies of Test Effectiveness. In Proceedings of the 6thACM SIGSOFT International Symposium onFoundations of Software Engineering, 153–162.
3. Phyllis G Frankl and Stewart N Weiss. 1993. An Experimental Comparison of the Effectiveness of Branch Testing and Data Flow Testing. EEE Transactions on SoftwareEngineering 19, 8: 774–787.
4. Laura Inozemtseva and Reid Holmes. 2014. Coverage is not strongly correlated with test suite effectiveness. In Proceedings of the 36th International Conference on Software Engineering - ICSE 2014, 435–445. https://doi.org/10.1145/2568225.2568271
5. Akbar Siami Namin and James H. Andrews. 2009. The influence of size and coverage on test suite effectiveness. In Proceedings of the eighteenth international symposium on Software testing and analysis - ISSTA ’09, 57. https://doi.org/10.1145/1572272.1572280

