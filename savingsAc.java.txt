package Bankingapp;

public class SavingsAccount extends Account
{
	public SavingsAccount(long accountNo, String holderName, double accountBalance,String DoorNo,String StreetName,String District,String State,int Pincode){
		super(accountNo,holderName,accountBalance,DoorNo,StreetName,District,State,Pincode);
		System.out.println("SavingsAccount is Successfully Created....!");
	}
	/*SavingsAccount class is inherite Account class SavingsAccount class is Sub class of Account class
	 *Account class is Super class of SavingsAccount class
	 *Account lass is a Abstract class it contains Abstract methods
	 *Abstract methods also inherited so we should declare class as Abstract or Override the abstract methods
	 *that is only way to solve the problem.
	 *so we are override the DepositeAmount() and WithdrawAmount().
	 */
	void DepositeAmount(double amount) {
	    AccountBalance=AccountBalance+amount;
		System.out.println("Your Deposite amount : "+amount);
		System.out.println("Your Total Account Balance : "+AccountBalance);
	}
	void WithdrawAmount(double amount) {
		 AccountBalance=AccountBalance-amount;
	     System.out.println("Your Withdraw amount : "+amount);
		 System.out.println("Your Total Account Balance : "+AccountBalance);
	}
}