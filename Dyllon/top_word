def top_words(text, n):
    import re
    from collections import Counter

    # Normalize the text to lowercase and remove punctuation
    text = text.lower()
    text = re.sub(r'[.,!?;:]', '', text)

    # Split the text into words
    words = text.split()

    # Count the frequency of each word
    word_counts = Counter(words)

    # Get the n most common words, sorted by count and then alphabetically
    most_common = word_counts.most_common()
    most_common.sort(key=lambda x: (-x[1], x[0]))

    return most_common[:n]