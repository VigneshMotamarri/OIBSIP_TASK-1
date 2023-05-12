# OIBSIP_TASK-1
Online_ReservationSystem
import java.util.Scanner;  // Scanning Inputs 
class Reservation1 
{
    public static void main(String[] args)
    {
        //Initial Details of the user..!
        Scanner intake = new Scanner(System.in); // Creating Obj
        System.out.println("Welcome to the ONLINE RESERVATION SITE");

        System.out.print("Enter your Name\n");
        String name = intake.nextLine();    //Taking Them into a variable
        System.out.print("Enter your DoB\n");
        String DoB = intake.nextLine();
        System.out.print("Enter your phoneno\n");
        String phoneno = intake.nextLine();
        System.out.print("Enter your emailid\n");
        String emailid = intake.nextLine();
        System.out.println("User Name is:  " + name + " " + "User Date of Birth is : " +DoB);
        System.out.println("User Contact number: " +phoneno+ " " + "User EmailId is: "+emailid);
        //Login form
        System.out.print("Enter your Name\n");
        String name1 = intake.nextLine();
        System.out.println("Enter Your password\n");
        String password = intake.nextLine();
        if(name1==name&&password==DoB)
        {
            System.out.println("Hello User");
            System.out.println("User Name is:  " + name + "User Date of Birth is : " +DoB);
            System.out.println("User Contact number: "+phoneno+ "User EmailId is: "+emailid);
            System.out.println("Enter Your trainName: ");
            String trainName = intake.nextLine();
            System.out.println("Enter your trainNum: ");
            String trainNum = intake.nextLine();
            System.out.println("Enter Your trainClass: ");
            String trainClass = intake.nextLine();
            System.out.println("Enter Your Date of Journey: ");
            String trainJourney = intake.nextLine();
            System.out.println("Enter your startingplace: ");
            String trainStartingplace = intake.nextLine();
            System.out.println("Enter Your Destination: ");
            String trainDestination = intake.nextLine();
            System.out.println("Enter Your Time of Journey: ");
            String trainTime = intake.nextLine();
            System.out.println("Ticket Will be sent to your Contact number and EmailId");
        
            // Cancel reservation
            System.out.print("Do you want to confirm cancellation? (y/n): ");
            String confirmation = intake.nextLine();
            if (confirmation.equalsIgnoreCase("y")) 
            {
            System.out.println("Reservation cancelled.");
            System.out.println("Thank You");

            }   
            else
            {
            System.out.println("Cancellation not confirmed.");
            System.out.println("Check Your details Once");
            System.out.println("User Name is:  " + name + " " + "User Date of Birth is : " +DoB);
            System.out.println("User Contact number: " +phoneno+ " " + "User EmailId is: "+emailid);
            System.out.println("Happy Journey");
            }
        }
    }
    
}
