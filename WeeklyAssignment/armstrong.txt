package assignments;

public class Armstrong1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int num=1634;
		int original=num;
		int NoOfDigits=0;
		int armstrong=0;
	
		for(;num>0;)//15
		{
			NoOfDigits++;
			num=num/10;
		}
	
		num=original;
		for(;num>0;)
		{
			
			int lastdigit=num%10;
			int multiply=1;
			for(int i=1;i<=NoOfDigits;i++)
			{
				multiply=multiply*lastdigit;
				
			}
			armstrong=armstrong+multiply;
			num=num/10;
		}
		System.out.println("armstrong result: "+armstrong);
	
	}

}
