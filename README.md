# Insertion-Sort-
class SelectionSort{
    public static void main(String[] args) {
        int arr[]={99,10,3,-1,0,6,2,1};
        int n=arr.length;
        System.out.println("Array before Sorting");
        System.out.println(Arrays.toString(arr));
        for (int i=0;i<n;i++){
            int min=i;
            for (int j=i+1;j<n;j++){
                if (arr[j]<arr[min]){
                    min=j;

                }
            }
            if (min!=i){
                int temp=arr[min];
                arr[min]=arr[i];
                arr[i]=temp;

            }
        }
        System.out.println("Arrays after sorting");
        System.out.println(Arrays.toString(arr));
    }
}
