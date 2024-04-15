# sentence-analysis
Algorithm SentenceAnalysis(sentence)
    Input: sentence (a string representing the sentence ending with a period)
    Output: length (an integer representing the length of the sentence)
            wordCount (an integer representing the number of words in the sentence)
            vowelCount (an integer representing the number of vowels in the sentence)

    length := 0
    wordCount := 0
    vowelCount := 0

    For each character in sentence:
        If character ≠ ' ' AND character ≠ '.':
            length := length + 1

        If character = ' ':
            wordCount := wordCount + 1

        If LowerCase(character) ∈ {'a', 'e', 'i', 'o', 'u'}:
            vowelCount := vowelCount + 1

    wordCount := wordCount + 1  // accounting for the last word

    Output length, wordCount, and vowelCount
