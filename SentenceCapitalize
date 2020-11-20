def main():
    my_string = input("Enter a string and I will capitalize the first letter of every sentence: ")
    capitalize(my_string) # pass my_string for capitalization
def capitalize(my_string):
    try:
        my_string_list = []
        for char in my_string: # add every character in my_string into a list of char
            my_string_list.append(char)
        my_string_list[0] = my_string_list[0].upper() # first letter of the string should be capitalized regardless

        length = len(my_string_list) # size of list
        position = 0 # current index within list
        for char in my_string_list:
            if length - position == 2: # this will prevent an IndexError when sentences end with ., ?, or !
                break
            if char == "." or char == "?" or char == "!": # if sentence ends with ., ?, or !
                my_string_list[position + 2] = my_string_list[position + 2].upper() # capitalize the first letter following
            position += 1 # increment position
        my_new_string = ""
        for char in my_string_list: # convert the character list to a string
            my_new_string += char
        print(my_new_string)
    except IndexError:
        print("Index out of range")
main()
