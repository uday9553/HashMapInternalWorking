# HashSetInternalWorking

# Internal Working of HashMap

# it follows Bucket format. it has 16 buckets(Buckets are indexed from 0 to 15).

and each bucket has a Linked List

# Each Linked List has 4 attributes/values i.e hashcode, key, value, next_node_address

 
# when trying add new element using put() method. it first takes key and compute hashcode() and then do some modular operation with hashcode of the key to get bucket index and place the values in the bucket having LinkedList(hashcode,key,value,address).

# If we get hashcollision i.e we get same hashcode multiple times then it will create new LinkedList at the same bucket and point this node address to previous node.

# If we give null as a key for map then in which bucket it will store?
Ans : It will store at 0 index bucket

# when trying add new element using put() method. it first takes key and compute hashcode() and then do some modular operation with hashcode of the key to get bucket index and place the values in the bucket having LinkedList(hashcode,key,value,address).

# If we get hashcollision i.e we get same hashcode multiple times then it will create new LinkedList at the same bucket and point this node address to previous node.

# If we give null as a key for map then in which bucket it will store?
Ans : It will store at 0 index bucket

# Adding Values to map(using put method)
1.when we are trying to add new Elements it will be placed in buckets.
2.before placing it in the buckets it will see threshold value. if it is exceeding load factor(75%) then the bucket size will be doubled
