# UserPass
package userpass;

import java.util.Scanner;

public class Main {

	public static void main(String[] args) {

		String username, password, answer = "", newpassword;
				
		Scanner inp = new Scanner(System.in); 
				
		System.out.println("Enter your username:");
		username = inp.nextLine(); 
				
		System.out.println("Enter your password:");
		password = inp.nextLine();

		if(username.equals("gamzedelil") && password.equals("gamze123")) {
			System.out.println("You are logged in."); }	
		
		else { 
			System.out.println("Your password is incorrect. Do you want to reset your password? (Please write Yes or No.)");
			answer = inp.nextLine(); }
		switch (answer) {
        case "Yes" :
            System.out.println("Enter your new password.");
            newpassword = inp.nextLine();

            if (newpassword.equals("gamze123")) {
                System.out.println("Your new password cannot be the same as the previous one.Try again.");
            } else {
                System.out.println("Your password has changed successfully.");
            }
            break;

        case "No" :
            System.out.println("Try logging in again.");
            break;

    }
  }
}

     
		
 
  
