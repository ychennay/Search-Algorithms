// code from Udemy course Practical Data Structures and Algorithms by Imtiaz Ahmad. His course is amazing and I highly recommend it.

package insertionSort;
import java.util.Arrays;
import java.util.Scanner;

public class App {

public static void main(String[] args){

    System.out.println("Please enter how many integers in the array to sort:");
    Scanner input = new Scanner(System.in);
    int sizeArray = input.nextInt();
    int[] inputArray = new int[sizeArray];

    for (int i = 0; i < inputArray.length; i++){

        System.out.println("Please enter the integer in position " + i + " of " + (sizeArray - 1) + ":");
        int inputValue = input.nextInt();
        inputArray[i] = inputValue;
    }

    System.out.println("Using Insertion Sort to sort the following array: " + Arrays.toString(inputArray));
    System.out.println("Final sorted array: " + Arrays.toString(insertSort(inputArray)));
}

public static int[] insertSort(int[] inputArray){

    for (int index = 1; index < inputArray.length; index++){
        int laggingIndex = index - 1;
        int specificVar = inputArray[index];

        while (inputArray[laggingIndex] > specificVar && laggingIndex > 0){

            inputArray[laggingIndex + 1] = inputArray[laggingIndex];

            laggingIndex--;

        }
        inputArray[laggingIndex + 1] = specificVar;
    }

    return inputArray;
}
}

