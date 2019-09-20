# second_largest

package elclipse;

public class second_largest {

	public static void main(String[] args) {


		int a[]= {1,2,3,4,5,6,7,8,909,110};
		int max=a[0],max1=Integer.MIN_VALUE;
		for(int i=1;i<a.length;i++) {
			if(max<a[i]) {
				max1=max;
				max=a[i];
			}
			else {
				if(max1<a[i] && a[i]!=max) {  //comparing element
					max1=a[i];
				}
			}
		}
		System.out.print(max1);
	}
}

/////time complexity is O(n^2)
