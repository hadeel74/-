public class Hello {
    static int []x=new int[3];
    public static void print(){
        System.out.print("[");
        for (int i = 0; i <x.length ; i++) {
            if(i==x.length-1)
                System.out.print(x[i]);
            else
                System.out.print(x[i]+",");

        }
        System.out.print("]");
    }
    public static void input(){
        Scanner s = new Scanner(System.in);

        for (int i = 0; i < x.length; i++) {
            x[i] = s.nextInt();

        }
    }
    public static void main(String[] args) {
       input();
        print();
    }
}
