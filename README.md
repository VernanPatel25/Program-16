class Library
{
    int acc_num;
    String title, author;
    int fine;
    void input(int acc,String t,String a)
    {
        acc_num = acc;
        title = t;
        author = a;
    }
    void compute(int days)
    {
        fine = (days*2);
        System.out.println("The no. of days late is "+days+". So, fine is "+fine+" Rs.");
    }
    void display()
    {
        System.out.println("Accession Number \t   Title  \t Author");
        System.out.println(acc_num+"   \t  " + title+"   \t  "+ author);
    }
    public static void main()
    {
        Library obj = new Library();
        obj.input( 1234, "Becoming", "Michelle Obama");
        obj.compute(6);
        obj.display();
    }
}
