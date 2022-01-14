public class singleton {

   private static singleton instance = null;
   private singleton() {
      // Exists only to defeat instantiation.
   }

   public static singleton getInstance() {
      if(instance == null) {
         instance = new singleton();
      }
      return instance;
   }
   public void getcontactdetails()
   {
	   System.out.println("Contact details");
   }
   public static void main(String[] args)
   {
	 singleton sing1=singleton.getInstance();
	 System.out.println(sing1);
	 sing1.getcontactdetails();
   }
}
