  # Calculator-
A calculator using HTML, JavaScript and CSS
  # How it Functions:

The calculator is composed of a display area and buttons to preform specific functions.

  <input type="text" name="display" readonly>
- This filed shows the numbers and operations as the user interacts with the calculator. 
- The “readonly” attribute makes it so no values can be typed into the display div

Each button tiggers a JavaScript action through the "onclick" attribute.
-	Clicking a number button adds the value to the display filed.
-	Example:
		Initial: display.value = ""
		Clicking "7": display.value='7'
		Clicking "5": display.value='75'

The “AC” button sets the display.value to an empty string
The “DEL” button uses “.slice(0, -1)” to remove the last character
The “=” button, evaluates the entire expression in the disblay by using the eval() function. And updates the display.value

In conclusion,
- User clicks buttons:
  The onclick attribute updates the display.value with numbers, operators, or results.
- Mathematical operations:
  Numbers and operators are added to display.value as a string (e.g., "7+5").ss,
  The "=" button runs “eval()” on this string to calculate the result.
- Result is displayed:
  The result replaces the current expression in the display field.
