# flow-reliability-computation

Code developed in CS:2820, Introduction to Software Development during the Fall 2024 semester at the 
University of Iowa. Working in groups of five, we implemented missing classes and debugged existing 
code to successfully compute flow reliability through determining if a schedule meets all of its 
given requirements. 

# CS2820 Fall 2024 WARP Project Code

This code base will be used for the University of Iowa CS 2820 Introduction to Software
Development course. The code was developed by Steve Goddard for the WARP sensor network 
research project. It was first written in Swift and rewritten in Java. It was then 
rewritten again in an object-oriented programming style. It was a quick
hack, and it needs a lot of cleanup and refactoring. A perfect code base to teach
the value of software development fundamentals!
<br>
<br>
Adding arguments to the Run Configuration allows you to execute more with your code. 
-i gives an input file and -o an output. -v is verbose, -sch priority is the priority 
scheduler, and --all runs all options. Whenever using --all, you will want to use -sch 
priority or change Warp to not run every option in the --all, otherwise, you will end up 
with a load of files. 
<br>

# Sprint3

Teagan Andrews, Manthan Shah, Katelyn Lookingbill, Victoria Delgado, and Molly Patterson worked in collaboration to complete the third and final sprint of the final project for CS:2820.

Teagan Andrews, Manthan Shah, and Katelyn Lookingbill used pair programming techniques to **implement getReliabilities and verifyReliabilities methods** in the ReliabilityAnalysis class with the assistance of helper methods. This implementation allows ReliabilityVisualization to create the output table of probabilities. 

Molly Patterson **wrote JavaDoc comments** for all attributes, methods, and constructors in ReliabilityAnalysis and **fixed formatting errors** with CheckStyle to ensure that our code matches the style guide for this class. 

Victoria Delgado, Katelyn Lookingbill, and Molly Patterson **developed JUnit test cases** for newly implemented methods in ReliabilityAnalysis class.

Katelyn Lookingbill **updated the README file** to include each member's tasks for Sprint3 and to ensure every artifact can easily be found.

Molly Patterson **updated the sequence diagram** to account for changes made in ReliabilityVisualization class, as we did not do this in Sprint2. 

Katelyn Lookingbill **updated the UML class diagram** of ReliabilityVisualization class to match updates to the createColumnHeader method. She also **populated a new UML class diagram** for ReliabilityAnalysis class to reflect new methods.

All necessary files including our **project plans,** **UML class diagrams of ReliabilityVisualization and ReliabilityAnalysis** with updates from Sprint3, a **sequence diagram** of warp processing the -ra flag with updates to ReliabilityVisualization can all be found in the **ARTIFACTS** folder inside of the Sprint3 branch. 

**Tests** for new methods in ReliabilityAnalysis can be found in the **test** folder in the ReliabilityAnalysisTest.java file. 

# Sprint2

The collaboration of Molly Patterson, Teagan Andrews, Victoria Delgado, Manthan, Shah, 
and Katelyn Lookingbill ensured the completion of the second sprint of the final project
for CS:2820. 

Manthan Shah, Victoria Delgado, and Katelyn Lookingbill used pair programming techniques to 
**implement the ReliabilityVisualization class.**

Teagan Andrews, Manthan Shah, and Molly Patterson **developed JUnit test cases** for the newly implemented 
methods in ReliabilityVisualization class.

Molly Patterson **wrote JavaDoc comments** for all attributes, methods, and constructors in 
ReliabilityVisualization class.

The entire team collaborated to **update the UML class diagram and sequence diagram,** accounting
for our updates to ReliabilityVisualization. 

Katelyn Lookingbill **updated the README file** to include the tasks of Sprint2 and where files 
are located. 

Victoria Delgado **updated the project plans** document to reflect who completed what tasks
and the order that they were completed.

All necessary files including **project plans,** **a UML class diagram of ReliabilityVisualization,** 
including an updated version from Sprint2, and an **updated sequence diagram** of warp processing
the -ra flag can be found in the **ARTIFACTS folder** inside the Sprint2 branch. **Tests** for methods
in the ReliabilityVisualization class are found in the **test folder** in the 
ReliabilityVisualizationTest file.


# Sprint1

Molly Patterson, Teagan Andrews, Victoria Delgado, Manthan Shah, and Katelyn Lookingbill
collaborated to complete the first sprint of the final project for CS:2820. Our team
made a sequence diagram displaying the interactions between Warp classes starting with
processing the "ra" instruction. Our team met two different times to pair program. 
We found a website called draw.io where we could work on the same diagram simultaneously.
Katelyn Lookingbill created a UML Diagram with Visualization to serve as a visual
supplement to our understanding of the classes' and methods' interactions. Manthan Shah
managed a document detailing our plans, requirements, and expectations for working on the
project. All group members gave input when deciding what to include in the document. While
working on the diagram, each member added their own edits. Ideas were discussed before 
implementation. All necessary files were placed in the Artifacts folder in the Sprint1 branch. 




## Homework 5: Refactoring WorkLoad Methods in the ReliabilityAnalysis Class

Manthan Shah, Molly Patterson, and Katelyn Lookingbill refactored the 
getFixedTxPerLinkAndTotalTxCost and numTxAttemptsPerLinkAndTotalTxAttempts
methods from the WorkLoad class in the WARP package. The methods' functionalities
were consolidated into the numTxPerLinkAndTotalTxCost method in the
ReliabilityAnalysis class. The method results in the output of either
WorkLoad method based on which helper method is used. Katelyn and Molly
wrote the helper method for numTxAttemptsPerLinkAndTotalTxAttempts, Manthan
wrote the helper method for getFixedTxPerLinkAndTotalTxCost and 
numTxPerLinkAndTotalTxCost, and all three worked on JavaDoc comments,
WorkLoad instantiation, and formatting.
 
Java Doc comments made by jcbates: Workload.java, Flow.java, ProgramVisualization, and Program.java
<br>
<br>
Java Doc comments made by klookingbill: Warp.java and VisualizationImplementation.java  
10/8/2024
<br>
# **Junit Tests Completed by jcbates:**
### Tests for setFlowDeadline()
testSetFlowDeadlineUpdateExistingFlow 
<br>testSetFlowDeadlineValidFlow

### Tests for getFlowDeadline()
<br>testGetFlowDeadlineInvalidFlow
<br>testGetFlowDeadlineValidFlow

### Tests for testMaxFlowLength()
<br>testMaxFlowLengthNoFlows 
<br>testMaxFlowLengthStressTest4

### Tests for getHyperPeriod()
<br>testGetHyperPeriodEmptyFlow
<br>testGetHyperPeriodValidFlows

### Tests for getNodesInFlow()
<br>testGetNodesInFlowNullFlow 
<br>testGetNodesInFlowNonExistentFlow
<br>testGetNodesInFlowValidFlowF1 

### Tests for getNodesInFlow()
<br>testGetNodeIndexExistingNode
<br>testGetNodeIndexNonExistentNode

### Tests for getFlowNames()
<br>testGetFlowNamesEmpty
<br>testGetFlowNames
<br>
<br>
# **Junit Test Completed by klookingbill:**
### Tests for addFlow()
These tests check that the method can successfully add a non-existing flow to "StressTest4.txt" file, add a pre-existing flow to the file, and add multiple new flows to the file. 
<br>
<br>addFlowAddTest
<br>addFlowOverridingTest
<br>addFlowMultipleAddsTest
### Tests for addNodeToFlow()
These methods tests that a node that already exists in the "StressTest4.txt" file can successfully be added to a flow and that a node that does not already exist in the file is also correctly added to a flow.
<br>
<br>addNodeToFlowExistsTest
<br>addNodeToFlowDoesntExistTest
### Tests for getTotalTxAttemptsInFlow()
These tests check that the total transmission attempts is correctly calculated for a single flow and for multiple nodes. 
<br>
<br>getTotalTxAttemptsInFlowOneFlowTest
<br>getTotalTxAttemptsInFlowMultiFlowsTest
### Tests for getFlowPriority()
Because of the simplicity of this method, I have one test that makes sure the priority of a specified node is correctly computed.
<br>
<br>getFlowPriorityTest
### Tests for setFlowPriority()
My test checks that the priority of the given node is equal to the input of the given priority.
<br>
<br>setFlowPriorityTest
### Tests for getFlowTxAttemptsPerLink()
These tests check that the method correctly finds the priority of the specified flow and that it will also find the correct priority of an empty flow.
<br>
<br>getFlowTxAttemptsPerLinkTest
<br>getFlowTxAttemptsPerLinkEmptyTest
### Tests for setFlowsInRMorder()
One of my tests checks that the method correctly orders the flows in a given file with just the flows in the file. The second test checks that the method still accurately orders the flows even when adding in new flows.
<br>
<br>setFlowsInRMorderCorrectOrderTest
<br>setFlowsInRMorderAddFlowsTest
### Tests for getNodeNamesOrderedAlphabetically()
My first test ensures that the method correctly orders the initially existing flows in the file in alphabetical order. The second test checks that the method still orders correctly even when adding in new flows to the file. 
<br>
<br>getNodeNamesOrderedAlphabeticallyTest
<br>getNodeNamesOrderedAlphabeticallyAdditionalFlowsTest
<br>
<br>
### 10/15/24
# UML Diagrams
<br>
I used UML Lab to create UML diagrams for classes: SchedulableObject, WorkLoad, and the third diagram shows all of the Reliability classes.
<br>

### SchedulableObject
The SchedulableObject model maps out all of this class's children and public elements. I was able to create a model with these specifications by 
hiding the non-public elements from the model. 
<br>

### WorkLoad
The WorkLoad model not only shows the WorkLoad class methods, but it also entails its parent classes and associated classes. This model shows all
elements, no matter their visibility level - public or private. The WorkLoad model has significantly more elements becausTThee of the numerous parent
and associated classes. 
<br>

### Reliability
The final model shows not just one class but rather all of the Reliability*.java classes. With the different classes in the model, I then added in 
the parent classes and associated classes only for the ReliabilityVisualization class. For the ReliabilityAnalysis class, I added in a new public 
method titled, getReliabilities, that returns a Reliability Table. I then generated code from this which added the method to the 
ReliabilityAnalysis.java file. 
<br>
