# Flower-Shop-Java

import java.util.*;
public class FlowerShop {
	public static void main(String[] args){
		
		String flower;
		int individual;
		String receiver;
		int n1;
		Scanner keyboard = new Scanner(System.in);
		
		System.out.println("Welcome to the Flower shop!");
		System.out.println("What type of flowers would you like to buy?");
		flower = keyboard.nextLine();
		
		if(flower.equalsIgnoreCase("roses")){
			System.out.println("How many dozen roses would you like to purchase?");
		individual = keyboard.nextInt();
		System.out.println("You are going to purchase " + individual * 12 + " individual roses.");
		}
		
		else if(flower.equalsIgnoreCase("lilies")){
			System.out.println("Who are the lilies for?");
		receiver = keyboard.nextLine();
		n1 = receiver.length();
			if (n1 <= 5) {
			System.out.println("The receiver of these flowers has a short name.");
			}
			else if (n1 > 5) {
			System.out.println("The receiver of these flowers has a long name.");
		}
		}
			
		else {
			System.out.println("Unfortunately, we do not carry that type of flower.");
		}
		System.out.println("Thank you for visiting the Flower Shop!");
		}
	}

