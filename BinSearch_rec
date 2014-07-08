def Binary_Search(my_Array,num_to_search,first,last):
#    first = 0
 #   last = len(my_Array) - 1
    if (last < first):
       return False
    else:
       middle = (first + last)//2
       if(my_Array[middle]< num_to_search):
        first = middle + 1
        last = len(my_Array) - 1

        return Binary_Search(my_Array,num_to_search,first,last)
       elif(my_Array[middle]> num_to_search):
        first = 0
        last = middle-1
        return Binary_Search(my_Array,num_to_search,first,last)
       elif(my_Array[middle] ==num_to_search):
        
        return True

if __name__ == "__main__":
    my_Array_S = []
    my_Array = []
num_of_numbers = int(input('Number of elements in sorted array? '))

for i in range(0, num_of_numbers):
   my_numbers = int(input('Number to be added to array: '))
   my_Array_S.append(my_numbers)

#why this step? You can convert them to int when you get them in the input itself no?
my_Array = list(map(int, my_Array_S))
# ====
first = 0
last = len(my_Array) - 1

num_to_search = int(input("Number to be searched in the Sorted Array?"))
if num_to_search not in my_Array:
    print("False")
    exit()
else:

    if Binary_Search(my_Array,num_to_search,first,last):
	    print("Found!")
    else:
	    print("Nah!")
