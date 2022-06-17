# girilensayiyaEnKucukveEnBuyukYakinSayi
import java.sql.SQLOutput;
import java.util.Arrays;

public class Main {
    public static void main(String[] args) {


        int num = 5;

        int [] list ={15,12,788,1,-1,-778,2,0};

        int[] arrMin = new int[list.length];

        int[] arrMax = new int[ list.length];

        int a=0;
        int b=0;

        for(int i=0; i<list.length; i++){
            if(list[i]<=num){
                arrMin[a]=list[i];
                a++;
            }

            if(list[i]>=num){
                arrMax[b]=list[i];
                b++;
            }
        }

        int min =arrMax[0];
        int max = arrMin[0];

        for(int k:arrMax){
            if(k<min && k>num){
                min=k;
            }
        }

        for(int k:arrMin){
            if(k>max && k<num){
                max=k;
            }
        }

        System.out.println("Kucuk yakin number : "+ max);
        System.out.println("Buyuk yakin sayi : "+ min);



    }
}
