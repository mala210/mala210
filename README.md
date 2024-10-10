mkdir my-java-project
cd my-java-project
git init
touch Main.java
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/your-username/your-repo.git
git push -u origin master


// Java code for linearly searching x in arr[]. 
// إذا كان العنصر موجودًا، فسيتم إرجاع موقعه، وإلا سيتم إرجاع -1

class LinearSearch {
    // هذه الدالة تقوم بإرجاع فهرس العنصر x في المصفوفة arr[]
    static int search(int arr[], int n, int x) {
        for (int i = 0; i < n; i++) {
            // إرجاع فهرس العنصر إذا تم العثور عليه
            if (arr[i] == x)
                return i;
        }
        // إرجاع -1 إذا لم يتم العثور على العنصر
        return -1;
    }

    public static void main(String[] args) {
        int[] arr = {3, 4, 1, 7, 5}; // المصفوفة
        int n = arr.length; // طول المصفوفة
        int x = 4; // العنصر المطلوب البحث عنه
        int index = search(arr, n, x); // البحث عن العنصر في المصفوفة

        // طباعة النتائج
        if (index == -1)
            System.out.println("Element is not present in the array");
        else
            System.out.println("Element found at position " + index);
    }
}

// الاسم: [malath alsaeedi]
// الرقم التعريفي: [443002873]

