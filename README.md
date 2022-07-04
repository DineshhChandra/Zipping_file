# Zipping_file
Huffman algorithm is used for file compression without loosing any data
Huffman coding creates a tree using the frequencies of the character and then generates code for each character.
Once data is encoded, it has to be decoded and decoding is done using the same tree
Create a priority queue Q consisting of each unique character.
Sort them in ascending order of their frequencies.
for all the unique characters:
    create a newNode
    extract minimum value from Q and assign it to leftChild of newNode
    extract minimum value from Q and assign it to rightChild of newNode
    calculate the sum of these two minimum values and assign it to the value of newNode
    insert this newNode into the tree
return rootNode
