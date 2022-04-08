I'm doing a (free) operating system (just a hobby, won't be big and professional
like gnu) for 386(486) AT clones.

[1991-08-25, https://groups.google.com/g/comp.os.minix/c/dlNtH7RRrGA/m/SwRavCzVE7gJ]

…git actually has a simple design, with stable and reasonably well-documented
data structures. In fact, I'm a huge proponent of designing your code around the
data, rather than the other way around, and I think it's one of the reasons git
has been fairly successful […] I will, in fact, claim that the difference
between a bad programmer and a good one is whether he considers his code or his
data structures more important. Bad programmers worry about the code. Good
programmers worry about data structures and their relationships.

[2006-06-27, https://lwn.net/Articles/193245/]

I'm an egotistical bastard, and I name all my projects after myself. First
Linux, now git.

[2007-06-14]


import java.io.*;
import java.util.*;
class GFG {
    public static void main(String[] args)
    {
        // creating array list
        List<Integer> my_list = new ArrayList<>();
        my_list.add(10);
        my_list.add(20);
        my_list.add(30);
        my_list.add(40);
        my_list.add(50);
        my_list.add(60);
        my_list.add(70);
  
        // Printing list before rotation
        System.out.println(
            "List Before Rotation : "
            + Arrays.toString(my_list.toArray()));
  
        // Loop according to the number of rotations
        for (int i = 0; i < 4; i++) {
            // storing the first element in the list
            int temp = my_list.get(0);
            // traverse the list and move elements to left
            for (int j = 0; j < 6; j++) {
                my_list.set(j, my_list.get(j + 1));
            }
            my_list.set(6, temp);
        }
  
        // Printing list after rotation
        System.out.println(
            "List After Rotation :  "
            + Arrays.toString(my_list.toArray()));
    }
}


