package Bankingapp;

public class Address {
     public String DoorNo;
     public String StreetName;
     public String District;
     public String State;
    public int Pincode;
	public Address(String DoorNo,String StreetName,String District,String State,int Pincode) {
		this.DoorNo=DoorNo;
		this.StreetName=StreetName;
		this.District=District;
		this.State=State;
		this.Pincode=Pincode;
	}
}