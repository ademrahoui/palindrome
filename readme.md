# Palindrome Checker

## Overview

This repository contains a simple algorithm for checking whether a given word is a palindrome. The algorithm compares characters located at the ends of the word and proceeds as follows:

- If the characters at the ends are equal, it tests the rest of the word.
- If there is a difference, the algorithm stops.

The stop condition for the algorithm is as follows:

- An empty word or a word containing a single character is considered a palindrome.

## Algorithm

```pseudocode
FUNCTION IsPalindrome(word: string) RETURNS BOOLEAN
BEGIN
    // Stop condition
    IF length(word) <= 1 THEN
        RETURN TRUE
    END IF

    // Compare characters at the ends
    IF firstCharacter(word) = lastCharacter(word) THEN
        // Recursively check the rest of the word
        RETURN IsPalindrome(middleCharacters(word))
    ELSE
        RETURN FALSE
    END IF
END
```
