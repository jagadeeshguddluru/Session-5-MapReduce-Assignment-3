# Session-5-MapReduce-Assignment-3
package p;

public class Assingment {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		String line="Hadoop is open source frame work, Hadoop is good Frame work for handling big data";
		String s[]=line.split("\\W+");
		for (String k : s )
			System.out.println(k);
		
		for(int i=0;i<s.length;i++){
			int sum=1;	
			for(int j=i+1;j<s.length;j++){
				if(s[i].equalsIgnoreCase(s[j])){
					sum++;
					
				}
			}int x=0;
				for(int k=i-1;k>=0;k--){
					
					if(s[i].equalsIgnoreCase(s[k])){
						x++;
						
					}
				}
				if(x>0){
					//System.out.println();
				}
				else{
				System.out.println(s[i]+"      "+sum);
				}
			
		}
	}

}


output:

Hadoop
is
open
source
frame
work
Hadoop
is
good
Frame
work
for
handling
big
data
Hadoop      2
is      2
open      1
source      1
frame      2
work      2
good      1
for      1
handling      1
big      1
data      1
