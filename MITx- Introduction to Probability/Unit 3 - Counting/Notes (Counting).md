## Counting 

- Counting is useful because we often want to count the entire sample space and our event of interest. Many a times they can be large and it is useful to know some basic combinatorics.

- **The Counting Principle** : The total number of possible results of the r-stage process is n1 * n2 * n3 * ... n<sub>r</sub>.

- For e.g., to order an ice cream we have to choose from 2 cone types, 12 flavors and 7 toppings. So the total number of ways to order an ice cream is 2 * 12 * 7

- **Summary of Counting Results** 
    - **Permutations** of n objects: n!
    - **k-permutations** of n objects: n! / (n - k)!
    - **Combinations** of k out of n objects: n choose k = n! / k! (n - k)!
    - **Partitions** of n objects into r groups, with the i<sub>th</sub> group having n<sub>i</sub> objects: n! / n1 ! * n2 ! * n3 ! ..n<sub>r</sub> !

### Counting Examples 

#### Permutations

- A permutation of a set of objects is a way of ordering them.
- For example if we have 2 objects say 1, 2, there are two ways of ordering them <br/>
1 2<br/>
2 1

- For n objects, we have n! ways ... i.e., P<sub>N</sub> = N!

- An equivalent way of thinking about the P<sub>N</sub> = N! result is the following. For concreteness, let’s say that we have four people, Alice, Bob, Carol, and Dave. And let’s assume that they need to be assigned to four seats arranged in a line. The N! result tells us that there are 4! = 24 different permutations they can take.

- Number of subsets of {1, 2, 3, ..n} => Each element can be arranged to form a set with itself and the empty element. Therefore, for a set of n elements 2 * 2 * 2 * 2 ... 2 = 2<sup>n</sup>


#### Counting Examples
- Number of licence plates with two letters followed by three numbers -> 2 * 2 * 3 * 3 * 3

- Number of licence plates with two letters followed by three numbers -> 2 * 1 * 3 * 2 * 1



