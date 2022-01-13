package com.company;

public class account {
    int acc_no;
    String name;
    float amount;

    void insertAccount(int n, String nm, float amt) {
        acc_no = n;
        name = nm;
        amount = amt;
    }

    void display(){
        System.out.println("Account Number: "+acc_no+"\n Name: "+name+"\n Amount: "+amount);
    }

    void deposit(int amt1){
        amount=amount+amt1;
        System.out.println(amt1+" is deposited");
    }

    void withdraw(int amt2){
        amount=amount-amt2;
        System.out.println(amt2+" is withdrawn");
    }

    void checkBalence(){
        System.out.println("Balence is "+amount);
    }
}

class testAccount{
    public static void main(String[] args) {
        account a = new account();
        a.insertAccount(12061999,"Rushikesh kaikade", 28000);
        a.checkBalence();
        a.deposit(10000);
        a.checkBalence();
        a.withdraw(5000);
        a.checkBalence();
        a.display();

    }
}
