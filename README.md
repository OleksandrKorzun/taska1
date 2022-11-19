# taska1
taska = str(input("write liters A,B or C: "))

if taska == "A":
    list = input("Enter text for dictionary: ")
    splitWord = list.split()
    splitWord.sort()
    for word in splitWord:
        if word == word:
            print(str(word))

elif taska == "B":
    words = []
    a = input("Enter text for top 5 most reapeted words: ")
    words.extend(a.split())
    from collections import Counter
    counts = Counter(words)
    top5 = counts.most_common(5)
    print(top5)

elif taska == "C":
    def largestWord(s):
        s = sorted(s, key=len)
        print(s[-5:])
    s = input("Enter text for top 5 len words: ")
    l = list(s.split(" "))
    largestWord(l)
