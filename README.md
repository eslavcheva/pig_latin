# Pig Latin Challange

- Write a ruby script which converts a single word into pig latin
```ruby
# define a method called pig_latin that takes one argument
def pig_latin(word)
  # ...
end

# when the method is called it should return the word in pig latin
puts pig_latin("ruby")
# ubyray
```
- Pig latin is a game where words are converted into alternative versions according to a set of simple rules

## Pig Latin rules:

- For words beginning with one consonant, the consonant moves to the end, followed by *"ay"*<br>
Examples: <br>
"pig" => "igpay"
"latin" => "atinlay"
- For words beginning with vowel sounds, just add *"ay"* at the end<br>
Examples: <br>
"elevator" => "elevatoray"
- For words beginning with a consonant cluster, the whole cluster moves to the end, followed by *"ay"*<br>
Examples: <br>
"glove" => "oveglay"<br>
"where" => "erewhay"

## Tips and Hints:
- A consonant cluster is all letters before the first vowel
- Might be helpful to have an array of all the vowels
```ruby
VOWELS = ['a', 'e', 'i', 'o', 'u']
```
- A possible way to solve the challenge could be the following steps
```ruby
def pig_latin(word)
  # convert the word to an array
  # find first vowel position
  #   Array#find_index
  # if pos > 0
  # remove characters up to pos
  # return main + front + 'ay'
end
```

## Bonus Challenge

- Write methods that work together to convert a whole sentence into pig latin
- Use good capitalization
- Preserve punctuation
- Create a translator program by using a loop to get user input