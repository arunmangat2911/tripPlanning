# tripPlanning

import java.util.Scanner;
public class tripPlanning {
    public static void main(String[] args) {
        intro();
        budget();
        }
        public static void intro () {
            System.out.println("Welcome to Vacation Planner!");
            System.out.println("What is your name?");
            Scanner input = new Scanner(System.in);
            String name = input.nextLine();
            System.out.println("Nice to meet you " + name + " ,where are you travelling to?");
            String city = input.nextLine();
            System.out.println("Great! " + city + " sounds like a great trip");
        }

        public static void budget() {
            Scanner input = new Scanner(System.in);
            System.out.println("How many days are they going to spend in their destination?");
            int days = input.nextInt();
            System.out.println("How much money, in USD, are you planning to spend on your trip?");
            int money = input.nextInt();
            System.out.println("What is the three letter currency symbol for your travel destination?");
            String currency =  input.next();
            System.out.println("How many " + currency + " are there in 1 USD?");
            double count = input.nextDouble();
        }



    }

