package function;

public class Armstrong {
    public static void main(String[] args) {

        int n;
        System.out.println(isArmstrong(n= 111));

    }
    public static boolean isArmstrong(int n){
        int nod = countdigits(n);
        int on = n;
        int sum = 0;
        while(n > 0){
            int rem = n % 10;
            sum += Math.pow(rem,nod);
            n = n/10 ;


        }
        if( sum == on ){
            return true ;
        }
        else{
            return false ;
        }
    }
    public static int countdigits(int n){
        int nod = 0;
        while(n > 0){
            n=n/10;
            nod++;
        }


        return nod;
    }

}
