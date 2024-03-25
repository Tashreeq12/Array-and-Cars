
public class SumOfArrayElements {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        int[]array = {1,2,5,6,3,4};
        int sum = 0;
        
        for (int num : array){
        sum +=num;
        }
    System.out.println("Sum of all the elements in the array:" +sum);
            
    // Creating objects of Car and ElectricCar
    Car car = new Car("Toyota", "Yaris");
    ElectricCar myElectricCar = new ElectricCar("Telsa", "Model S", 120);
    
    // Displaying car details
    System.out.println("Toyota Yaris");
    System.out.println("Telsa Model S");
    
    }


    
}

public class Car {

    String brand ;
    String model;
   
   
    // Constructor to initiliaze brand and model
    public Car(String brand,String model)
    {
        this.brand = brand;
        this.model = model;
       
    }
   
    // Getter for brand
    public String getBrand() {
        return brand ;
    }

   
   
    // Setter for brand
    public void setBrand(String brand) {
        this.brand = brand;
    }
   
   
    //Getter for model
    public String getModel(){
        return model;
    }
   
    //Setter for model
    public void setModel(String model){
        this.model = model;
    }
 
   
    //Method to display brand and model of the car
    public void displayDetails(){
        System.out.println("Car brand:" + brand);
        System.out.println("Car model:" + model);
       
       
    
        }
       
    } 




    class ElectricCar extends Car {
    
    
    private double batteryCapacity; // in KWh
   
    //Constructor to initialize brand, model and battery capacity
    public ElectricCar(String brand, String model, double batteryCapacity){
        super(brand, model);
        this.batteryCapacity = batteryCapacity;
    }
   
    // Overriding displayDetails() method to include battery capacity
    @Override
   
    public void displayDetails(){
        super.displayDetails();
        System.out.println("Battery Capacity: " + batteryCapacity + " kWh");
    }
   
    //Main method for testing
    public static void main(String[] args) {
        // Create an ElectricCar object
        ElectricCar myElectricCar = new ElectricCar("Telsa", "Model S", 120);
       
        // Display details of the electric car
        System.out.println("Details of the electric Car: ");
        myElectricCar.displayDetails();
       
    }
       
       
    }
    




