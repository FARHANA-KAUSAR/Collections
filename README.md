# Collections
import java.util.*;
import java.io.*;
public class Collections{
    public static void main(String []args) throws Exception{
    ArrayList<Integer> al=new ArrayList<Integer>();
    al.add(10);
    al.add(8);
    al.add(2);
    al.add(7);
    al.add(1);
    al.add(9);
    al.add(3);
    al.add(4);
    al.add(6);
    al.add(5);
    int s=1,pos,ele,opt;
    BufferedReader br =new BufferedReader(new InputStreamReader(System.in));
    while(s==1)
    {
        System.out.println("  Fetch=1 || add=2 || remove=3 || print=4  ");
        System.out.print("Enter the operation you want to perform: ");
        opt= Integer.parseInt(br.readLine());
        if(opt==1)
        {
            System.out.println("enter the position of element to be fetched: ");
            pos=Integer.parseInt(br.readLine());
            System.out.print(al.get(pos));
        }
        else if(opt==2)
        {
            System.out.println("Enter element to be added: ");
            ele=Integer.parseInt(br.readLine());
            System.out.println(al.add(ele));
        }
        else if(opt==3)
        {
            System.out.println("Enter element to be removed");
            ele=Integer.parseInt(br.readLine());
            System.out.println(al.remove(ele));
        }
        else
        {
            System.out.println("Printing elements:");
            for(Integer i:al)
            System.out.print(i+" ");
        }
        System.out.println("Want to quit=1/0 :: ");
        s=Integer.parseInt(br.readLine());
    }
     }
}
