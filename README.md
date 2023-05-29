import java.util.*;

public class remove {
    
    public static void main(String[] args) {
        // Create an array of letters and numbers with some duplicates
        Object[] values = {'a', 'a', 'b', 'b', 1, 2, 3, 2, 1, 1};

        // Convert the array to a list
        List<Object> list = Arrays.asList(values);

        // Create a HashSet object with the list to automatically remove duplicates
        Set<Object> set = new HashSet<>(list);

        // Convert the HashSet object back to an array without duplicates
        Object[] newArray = set.toArray();

        // Print the resulting array without duplicates
        System.out.print("Array without duplicates: " + Arrays.toString(newArray));
    }
}
