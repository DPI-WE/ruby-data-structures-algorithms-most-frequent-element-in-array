# Find the Most Frequent Element in an Array

## The problem
Write a method that:

Takes an array of integers as input.
Returns the most frequently occurring element in the array.
If there are multiple elements that appear a maximum number of times, return any one of them.

## Understand the Problem
Let's warm up with a simpler task to become comfortable with frequency analysis in an array.

- Consider the array [1, 2, 3, 2]. Identify the most frequently occurring element.
- 1
  - Not quite. 1 only occurs once. Is there another more frequent element?
- 2
  - That's right! The element 2 occurs twice in this array.
- 3
  - Not quite. 3 only occurs once. Is there another more frequent element?
{: .choose_best #identify_most_frequent_element title="Consider the array [1, 2, 3, 2]. Identify the most frequently occurring element." points="1" answer="2" }

This example should help you understand how to count occurrences of each element in an array.

## Think Aloud
During coding interviews, it's important to verbalize your thought process. Discuss your strategies, write pseudocode, and explain your approach. Starting with a simple solution and iterating towards a more elegant solution is a good strategy.

## Test your code
```ruby
arrays = [
  [1, 3, 2, 3, 4, 3],
  [10, 9, 8, 10, 10],
  [5, 5, 5, 6, 6, 6, 7]
]
array = arrays.sample
# Write your program using this method
def most_frequent_element(array)

end

puts most_frequent_element(array)
```
{: .repl #most_frequent_element title="Find the Most Frequent Element" readonly_lines="[1,2,3,4,5,6]"}

## Tips and Clues for Solving the Problem
- **Hash**: Use a hash to count the occurrences of each element. This method is efficient for tracking frequency.
- **Increment**: Increase the count of each element in the hash as you iterate through the array.
- **Find the Maximum**: Determine the element with the highest frequency by iterating through the hash.
- **Edge Cases**: Consider behavior for empty arrays. Ensure your solution handles various scenarios.

## Quiz
- What is the primary function of a hash in this problem?
- To count the occurrences of each element in the array.
  - Correct! Using a hash is an efficient way to keep track of how many times each element appears.
- To sort the array in ascending order.
  - Incorrect. While sorting can be useful for other problems, it's not the primary function of a hash in this context.
- To find duplicate elements in the array.
  - Incorrect, but close. While identifying duplicates is related, the primary function here is to count occurrences, not just to identify duplicates.
- To convert array elements into hash keys.
  - Incorrect. While array elements are used as hash keys, the main purpose is to count their occurrences, not just to convert them.
{: .choose_best #function_of_hash title="What is the primary function of a hash in this problem?" points="1" answer="1" }

- How should your function handle an empty array?
- Return nil
  - This is a valid approach. It's simple and conveys the absence of frequent elements.
- Return a predefined value or message
  - Also a valid option. It provides clarity to the user about the outcome.
- Raise an error
  - Appropriate in some contexts, especially if an empty array is considered an invalid input.
- Any of the above, depending on the implementation
  - Correct! The best approach depends on the specific requirements of your application and how you want to handle edge cases.
{: .choose_best #handle_empty_array title="How should your function handle an empty array?" points="1" answer="4" }

## Conclusion
In this lesson, we've tackled the challenge of finding the most frequent element in an array using hash maps for counting and array traversal. By breaking down the problem, employing a strategic approach with hash maps, and addressing edge cases, you
