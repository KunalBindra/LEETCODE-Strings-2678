# LEETCODE-Strings-2678
## Dry Run of `countSeniors`

### Understanding the Code
Before we start the dry run, let's break down what the code does:

- **`countSeniors(String[] details)`:** This method takes an array of strings as input, where each string represents a person's details.
- **`int c=0;`:** Initializes a counter `c` to store the number of seniors.
- **`for(int i=0;i<details.length;i++)`:** Iterates through each person's details in the array.
- **`String str=details[i].substring(11,13);`:** Extracts the age (two digits) from the current person's details.
- **`int age=Integer.parseInt(str);`:** Converts the extracted age string to an integer.
- **`if(age>60)`:** Checks if the person's age is greater than 60.
- **`c++;`:** If the age is greater than 60, increments the `c` counter.
- **`return c;`:** Returns the final count of seniors.

### Dry Run Example
Let's assume the following input array:

```
details = ["05/31/1969#Male#170#70", "05/31/1950#Male#180#70", "05/31/1994#Male#180#70"]
```

**Iteration 1:**
- `i = 0`, `details[i] = "05/31/1969#Male#170#70"`
- `str = "69"`
- `age = 69`
- `age` is not greater than 60, so `c` remains 0.

**Iteration 2:**
- `i = 1`, `details[i] = "05/31/1950#Male#180#70"`
- `str = "50"`
- `age = 50`
- `age` is not greater than 60, so `c` remains 0.

**Iteration 3:**
- `i = 2`, `details[i] = "05/31/1994#Male#180#70"`
- `str = "94"`
- `age = 94`
- `age` is greater than 60, so `c` becomes 1.

The loop ends.

**Final result:**
- `c` is 1, indicating there is one senior in the input array.

### Conclusion
The code effectively counts the number of seniors in the given array of details by extracting the age from each string, converting it to an integer, and checking if it's greater than 60.
 
**Note:** The code assumes that the age is always represented by two digits in the 11th and 12th positions of the input string. If the format of the input strings changes, the code might need adjustments.
 
**Would you like to try a different input array or explore potential improvements to the code?**
