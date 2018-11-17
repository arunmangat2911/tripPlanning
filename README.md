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
        int hour, minutes;
        hour = days * 24;
        minutes = days * 1440;
        System.out.println("If your are travelling for " + days + " days that is the same as " + hour + " hours or " + minutes + " minutes.");
        double spend;
        spend = money/days;
        System.out.println("If you are going to spend $" + money + " USD that means per day you can spend up to $" + spend + " USD");
        double total = money * count;
        double perday = total/days;
        System.out.println("Your total budjet in " + currency + " is " + total + " MXC, which per day is " + Math.round(perday) + " " + currency);

    }

    public static void time() {
        Scanner input = new Scanner(System.in);
        System.out.println("What is the time difference, in hours, between your home and your destination?");
        int timediff = input.nextInt();
        

    }


}


