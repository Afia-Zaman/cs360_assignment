def words_in_file(file_name):
    input_file = open(file_name, "r")
    contents = input_file.read().split()
    return set(contents)

def words_in_file2(file_name2):
    input_file2 = open(file_name2, "r")
    contents2 = input_file2.read().split()
    return set(contents2)


def main():
    file_name = input("File name: ")
    file_name2 = input("File name: ")

    words = words_in_file(file_name)
    words2 = words_in_file(file_name2)
    print(words, words2)

    union = words | words2
    print(union)

    difference = words2 - words
    print("Difference", difference)

    intersection = words.intersection(words2)
    print("Intersection: ", intersection)

    sym_diff = words ^ words2
    print("Sym difference:", sym_diff)

    if words <= words2:
        print("is the subset")

    if words.issuperset(words2):
        print("is a superset")


    word = input("add words: ")
    while word != "":
        words.add(word)
        word = input("add words: ")

    print(words)

    word = input("word: ")
    while word != "":
        words.discard(word)
        word = input("word: ")

    print(word)


    fruits = set(["lemon", "lime", "apple"])

    if "lemon" in fruits:
        print("make lemonade")

    if "orange" not in fruits:
        print("no orange juice")


    # DOESN'T WORK'
    for index in range(len(fruits)):
        print(fruits[index])

    for fruit in fruits:
        print(fruit)


    #
    fruits.remove("lime")
    print(fruits)

    fruits.remove("orange") # error
    print(fruits)

    fruits.discard("orange")
    print(fruits)

    fruits.clear()
    print(fruits)


    fruits.add("pear")
    print(fruits)

    fruits.add("lemon")
    print(fruits)

    fruits.update(["orange", "blueberry"])
    print(fruits)

    empty_set = set()
    print(empty_set)

    set1 = set([3.14, 5, "hello", "world"])
    print(set1)

    set2 = set([1, 3, 6, 6, 7, 7, 8])
    print(set2)

    set3 = set("fox")
    print(set3)

    set4 = set("raccoon")
    print(set4)

    even_numbers = set([-4, -3, 0, 2, 4])
    pos_number = set([0, 1, 2, 3, 4])

    all_numbers = even_numbers | pos_number
    print("Union: ", all_numbers)

    pos_even_numbers = even_numbers.intersection(pos_number)
    print("Intersection: ", pos_even_numbers)

    even_not_positive = even_numbers - pos_number
    print("Difference: ", even_not_positive)

    one_or_the_other = even_numbers.symmetric_difference(pos_number)
    print("Sym Difference", one_or_the_other)
main()
