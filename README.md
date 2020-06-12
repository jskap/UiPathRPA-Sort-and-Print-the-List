# UiPathRPA-Sort-and-Print-the-List
Sort the List and Print 3 Values. 
Given an input list of countries please sort the list and print the first 3 values in descending order.  

Note: Please use this value for the List initialization: new List(of String) from {"Germany", "Spain", "Japan", "Brazil", "India", "China"}.

In UiPath Studio, create a new project and use the following steps:

   1. Start the project as a sequence and define a List of Strings variable (“countries”) with the following default value: new List(of String) from {"Germany", "Spain", "Japan", "Brazil", "India", "China"}.
   2. Add an 'Invoke Method' activity and write 'Sort' under MethodName and “countries” under TargetObject. Leave the TargetType unchanged (null).
   3. Add an 'Invoke Method' activity. Write 'Reverse' under MethodName and have the other 2 fields just like in the previous 'Invoke Method'
   4. Print the extracted values using a 'Write Line' activity and the 'String.Join' and the ‘GetRange’ methods: String.Join (", ", countries.GetRange(0,3)).
   5. Add one more 'Invoke Method' activity.
   6.Type 'Reverse' in the MethodName field.
   7. In the TargetObject field, type the name of the original variable.
   8. Leave the TargetType unchanged (null).
   9. Create a new List of String variable.
  10. Add an 'Assign' activity to the Designer panel.
  11. In the To field, enter the variable created at step 11.
  12. In the Value field, enter the name of the original variable, followed by .GetRange(0,3). This variable stores the first three values in the sorted list.
  13. Print the extracted values using a 'Write Line' activity.
  14. Use the 'String.Join' method: String.Join (", ", secondvariablename.ToArray).
